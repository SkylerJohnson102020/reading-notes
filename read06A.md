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
                greetng = 'Good Evening!';
            } else if (hourNow > 12) {
                greeting = 'Good Afternoon!';
            } else if (hourNow > 0) {
                greeting = 'Good Morning!';
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
- The variable can be computed or calculated in the interpreter using the data that is temporarily stored in the var. 

[Back to Homepage](README.md)