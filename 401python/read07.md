# Python Scope

https://realpython.com/python-scope-legb-rule/

LEGB - Local, Enclosing, Global, and Built-in scopes

From the article:
> "Global scope: The names that you define in this scope are available to all your code.

> Local scope: The names that you define in this scope are only available or visible to the code within the scope."

Assignments, imports, function definition, args, and classes all involve their own scope.

from article:

> "Python scopes are implemented as dictionaries that map names to objects. These dictionaries are commonly called namespaces."

.keys() - returns the key names

### LEGB

An order in which Python views things. Looks from the inside to outside.

- **Local scope** - or function scope, this is the code block within a function or lambda expression.

- **Enclosing scope** - or nonlocal - special type of scope that exists only for nested functions.

From the article, VERY important point:
> "When you call outer_func(), you’re also creating a local scope. The local scope of outer_func() is, at the same time, the enclosing scope of inner_func(). From inside inner_func(), this scope is neither the global scope nor the local scope. It’s a special scope that lies in between those two scopes and is known as the enclosing scope. All the names that you create in the enclosing scope are visible from inside inner_func(), except for those created after you call inner_func()."

> "...names are resolved by first checking the local scope or the innermost function’s local scope."

- **Global scope** - or module scope - top level scope and is visible anywhere in your code

- Under the hood, Python will turn your code's main script into the module:

         __main__. 


This is the global scope of your program.

dir() - inspect names in your global scope

When you assign a value, you are either creating a new name or reassigning an existing name. A locally scope variable name will override the global variable with that same name.

Great code example from article:

            # This area is the global or module scope
        >>> number = 100
        >>> def outer_func():
        ...     # This block is the local scope of outer_func()
        ...     # It's also the enclosing scope of inner_func()
        ...     def inner_func():
        ...         # This block is the local scope of inner_func()
        ...         print(number)
        ...
        ...     inner_func()
        ...
        >>> outer_func()
        100

From the article:

> "Inside inner_func(): This is the local scope, but number doesn’t exist there.
> Inside outer_func(): This is the enclosing scope, but number isn’t defined there either.
> In the module scope: This is the global scope, and you find number there, so you can print number to the screen."


- **Built-in scope** - a scope that is created or loaded when a script is run. This also occurs when you open an interactive session. These are also available anywhere.

- A standard library module called "builtins".

- use dir() to view all of the built in options.

- use these built in modules as you would any other.

- you must import builtins.

- global statement - define a list of names that will have global treatment.

code example from article on how to use a global statement:

        >>> counter = 0  # A global name
        >>> def update_counter():
        ...     global counter  # Declare counter as global
        ...     counter = counter + 1  # Successfully update the counter
        ...
        >>> update_counter()
        >>> counter
        1
        >>> update_counter()
        >>> counter
        2
        >>> update_counter()
        >>> counter
        3

You can also create what is known as a lazy global name using a global statement. This is declaring a global variable inside a function. 

- nonlocal statement - similar with global, nonlocal names are accessible from inner funcs but are not assigned or updated.To modify, use nonlocal statement.

From article:

        >>> def func():
        ...     var = 100  # A nonlocal variable
        ...     def nested():
        ...         nonlocal var  # Declare var as nonlocal
        ...         var += 100
        ...
        ...     nested()
        ...     print(var)
        ...
        >>> func()
        200

> "With the statement nonlocal var, you tell Python that you’ll be modifying var inside nested(). Then, you increment var using an augmented assignment operation. This change is reflected in the nonlocal name var, which now has a value of 200.Unlike global, you can’t use nonlocal outside of a nested or enclosed function. To be more precise, you can’t use a nonlocal statement in either the global scope or in a local scope."

- you can't create lazy variables with a nonlocal statement.

[code401 Reading Notes](/401Python/code401Table.md)