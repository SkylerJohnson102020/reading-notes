# Javascript

Javascript is our third layer in a webpage where we can change the behaviour of the page, adding interactivity. Javascript enhances the user experience of the website and/or the experience of interacting with the website.

There are a few parts to a line of javascript code.

            document.write('Good Afternoon!');

- The first part of the code is the object. All browsers implement this object and you can use it simply by giving it's name here.
- An object can have many properties and methods, these are called members of that object. The dot, or member operator, helps us to access the members of the object named. You use the dot to access the members of a dot. 
- Method - the write() method of the indicated object, in this case document, gives us the ability the write new content to be written to our page where we have placed our script element. Make sure you open and close with the script element.
- Parameters - Our method may need some extra information or content in order for the method to work properly. We place this information in () just after the method. This piece of information can be more easily referred to as the parameter of the method. The js file needs to know what to write on the page. In the example above, the () contains 'Good Afternoon". 
**THERE ARE TWO PRIMARY PORTIONS OF OUR CODE, OBJECT AND METHOD.**

## JS and HTML

- When our browser comes upon a script element in the HTML code, it will stop on that script to load it and will also determine if it needs to do anything.
- We can place our script element anywhere we want in our html code. 
- The script element is set of instruction instructing that a particular computer will be able to follow in order one at a time. A single instruction is a **statement**. All statements should end with a ;.

#### Statements

            var today = new Date();
            var hourNow = today.getHours();
            var greeting;

            if (hourNow > 18) {
                greetng = 'Good Evening World!';
            } else if (hourNow > 12) {
                greeting = 'Good Afternoon World!';
            } else if (hourNow > 0) {
                greeting = 'Good Morning World!';
            } else {
                greeting = 'Welcome!';
            }

            document.write('<hjs>' + greeting + '</hjs>');

In the js example above you will see an example of a varied greeting. The lines beginning with var, greeting, and document are statements. The curly brackets indicate the beginning and end of a code block. The else if lines determines what code will run in this order. 

### **Statements** are one to a line, you must have only one statement per line and the statents are, in a nutshell, instructions. 

- Each one is a single instruction that the computer will follow. 
- Each one begins on it's own line and will end with a ;
- The semicolon is important at the end of your code since it will tell the js interpreter that the instruction is complete telling it to go onto the next instruction or step.
- **Code blocks** are statements that are contained with curly brackets. Each code block in the example above only contain one statment, the time. Code blocks are used frequently to contain multiple statements. Also, this makes it much easier to read your own code.
- You can write comments in your code to help better understand what the code is supposed to do.

 - ** Multi-Line comments** - These will encompass more than one line. Open with /*, write your text, then close with */.
- ** Single-Line comments** - Anything that you type past the // on that particular line will not be processed by the Javascript interpreter. These are used for what this line of code is doing. 

### **Variables**

- Variables are places where pieces of data can be stored temporarily from a script. 
- Once you leave a page, the data will be dropped from the browser memory. 
- The name, variable, is a good label for this idea since the data can change every time you visit the page and the script runs. 
- The variable can be computed or calculated in the interpreter using the data that is temporarily stored in the variable.

            var quantity = 3;

- **In the example above**, we have the keyword, var. (This keyword is used to create a particular variable.) The Javascript interpreter will understand that this keyword will create a variable. 
    - **var is the keyword**

    The variable name is, in this case, quantity.This is also known as an identifier. 
        
    - **The variable name is quantity.**

    _Note: If there is more than one word in your variable name, or identifier, you have to use what is called camelCase where any additional word is started with a capital. So, hourNow, camelCase, etc._

- The equals sign is the assignment operator. This example assigns a value to the variable. The 3 above is the variable value. If there is no value indicated, this variable is undefined.

#### JS identifies the differences between strings, numbers, and Booleans, which are true or false values.

 - **Numeric Data** handles numbers. You can only use characters 0-9. No commas are written in your numbers. You can also have negative numbers. Three quarters will be conveyed as 0.75

 - **String data** handles letters and and other characters. These can be used for any type of text. Use matching ' or " on wither side of your text. 

 - **Booleans** are true of false, on or off. For example, if an item is in stock or not, this is a true or false, yes or no value. 

 ## Six Rules for Naming Variables
1. The name needs to start with a letter, $, or _. Cannot start with a number.
2. The name of the variable can contain letters, $, or _. You cannot use a - or . in the name.
3. You are not allowed to use two things: reserved and keywords. See above for keyword definition. 
4. Variables are case sensitive. So, starting the same word uppercase and lowercase are two different variable names. It's not good methodically to use the same word for two different variables. 
5. Use like variable names for the information you are storing. 
6. Make sure you use camelCase when typing more than one word. 



            

[Back to Homepage](README.md)