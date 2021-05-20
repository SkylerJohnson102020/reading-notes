# Classes and Objects
https://www.learnpython.org/en/Classes_and_Objects

- An example from the article:

        class MyClass:
            variable = "blah"

            def function(self):
                print("This is a message inside the class.")

        myobjectx = MyClass()

myobjectx is holding an object of the "MyClass" class. This holds the function and variable contained within MyClass.

to access the variable:

        class MyClass:
            variable = "blah"

            def function(self):
                print("This is a message inside the class.")

        myobjectx = MyClass()

        myobjectx.variable
        myobjectx.function  #to access function

# Thinking Recursively
https://realpython.com/python-thinking-recursively/

From the article:

> "A recursive function is a function defined in terms of itself via self-referential expressions.This means that the function will continue to call itself and repeat its behavior until some condition is met to return a result."

- 2 parts: base case, recursive case.

From the article, a simpler recursive function using factorials:

        def factorial_recursive(n):
            # Base case: 1! = 1
            if n == 1:
                return 1

            # Recursive case: n! = n * (n-1)!
            else:
                return n * factorial_recursive(n-1)

Two things to consider when maintaining the state during recursion: (From Article:)

> "Thread the state through each recursive call so that the current state is part of the current call’s execution context."
> "Keep the state in global scope."

- READ ARTICLE AGAIN AND AGAIN



[code401 Reading Notes](/401Python/code401Table.md)