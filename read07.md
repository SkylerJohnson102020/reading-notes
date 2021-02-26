# Programming with JS

Examples of JS rely on the abilty to 

- **Access** content of a page
- **Modify** content of page
_ **Program** steps for a computer brower to take
- **React** to to event from the user implements in the browser.

1. **Define the Goal**

- What task to you want to achieve? Think of this as something you are giving to the computer to solve. 

2. **Design the Script**

- You need to design a series of steps that the computer will follow in order to find a solution to the puzzle. Use a flowchart to help visualize this.

3. **Code Each Step**

- Write the steps in a language the computer will understand. In this case, use Javascript.

**FLowcharts**
    - Flowcharts help visually show us how the script moves from one step to the next.

### Expressions

There are generally two types of expressions
1. The first type is just the expression will assign a value to the variable. So:

        -var color = 'blue';
        the value of color is blue

2. The second type uses two of more values, combines them, and returns one value. So:
    
        -var area = 2 * 6;
        The value of our area is now 12


### Operators
Operators are what expressions rely upon, they allow us to comnbine one to many values and create one value.

- **Assignment operators** the variable is assigned a value

        -color = 'blue';
        value of color is blue

- **Arithmetic Operators** calculcate simply math

        -area = 2 * 6;
        value of area is 12

Below is a list of operators:

        - + - adds a value to another value 
        - - - subracts a value from another value 
        - / - this will divide two values
        - * - multiples two values
        - ++ - increment, adds only one to current number. EX: i = 5, i++, the result is 11
        - -- - decrement, subtracts only one from current number. EX: i = 5, i--, result is 4
        - % - modulus, divides 2 values then returns what is left. 16 % 3, result is 1


- **String operators** Merge two strings

        greeting = 'Hello' + 'Skyler';
        value of greeting is Hello Skyler

- **Comparison operators** Merge two values and then return a true or false

        -buy = 5 > 10;
        false, value of by is false

- **Logical Operators** Merge expressions and will return either true or false

        -buy = (10 > 5) && (3 < 6);
        true, value of buy is true

- **Concatenation** - this is where we take two strings and merge them into one string. 

        let firstName = 'Skyler';
        let lastName = 'Johnson';
        let fullName = firstName + lastName;

**Functions**
Functions allow you to merge a collection or series of statements to perform a task. Functions make code reusable, the help avoid repeat code, allow us to define the code once then run it whenever we need it, and it allows your code to appear a lot cleaner. 

**Declaring** a function comes first. Declaring a function and **Invoking or, more commonly, Calling,** a function have to happen separately. Functions are invoked or called **by using ()**.

**Calling the Function**

- This is when you ask the function to perform it's designated task. 

**Parameters** 

- These are individual pieces of information the function needs in order to complete a task. Some functions require more than one piece of information, or parameter, to complete the task. The parameter inside a function behave like variable names.

**Return Value**

- When you expect the function to give you an answer.

#### A function holds a value, or information, and is only used when you are ready. Functions gather and hold information, then you have to **CALL** the function on the last line of the script. This will allow you to use the data the function gathered.

        function sayHello(){
            document.write('Hello');
        }

**In the example above:**

1. The function is "declared" by typing in the function keyword. 
2. You then give the function a name, or identifier. In this case, sayHello()
3. The curly brackets contain your statement. This will perform your task.
4. Using the function name in your code is how you are able to call the function.

### The steps of calling a function.
pg 91 diagram
1. The function stores the steps of a task.
2. When you require the script to execute your task, you then call the function.
3. The function will then perform the code written inside the curly brackets and put it on the website.
4. When it completes the task, the code will continue to run from where you called it.

**Sometimes your functions can seemingly be out of order and they might not work. (Example, you want the userName before the userName was declared.) This doesn't matter if the functions are all in the same script since the computer will run through the entire script before executing the statements.**

### Arguments

-**Arguments** are the values (parameters) held inside the the () of a function name. They can be presented as variables or values.

1. As a Value. (Ex below, 5 is width, 6 is height.)
            
            -getArea(5, 6); 

2. As a Variable. 

        wallWidth = 11;
        wallHeight = 17;
        getArea(wallWidth, wallHeight);


[Back to Homepage](README.md)