# Read 04 notes Links

**Links** You can create a tag using the a tag, or anchor element. Makes it a clickable link.

        <a href="url here">Website Title</a>

Generally you create a list comprised of of links, primarily for a links page or your nav bar. Usually in a ul.

**For an email**

    <a href="mailto:skyler@blah.com">Email Skyler</a>

**target** is an attribute used to open your link in a new window. To do this, set the value of target to _blank.

        <a href="url here" target="_blank">Website Title</a>

**Linking to spots on the same page** in the case that your page is long, you can add a list of links to jump to different portions of the page using the id att.
    
    <h1 id="top">Title</h1>
    <a href="#1st drop">1st drop</a>
    <a href="#2nd drop">2nd drop</a>
    <a href="#3rd drop">3rd drop</a>

    <h2 id="1st drop">1st drop</h2>
        some text here
        jjhdhsjkhfkashfjk
        asfhasjkhaklhfk
    <h2 id="2nd drop">2nd drop</h2>
        slkfasklfnsaklf
        ldknkssklsfkl
        slkdlksjkldsnfk
    <h2 id="3rd drop">3rd drop</h2>
        flashfljashfaljkh
        asklfhjalksfhslka
        aslkjfhakjfal
    <p><h2 href="#top">To Top</h2>


# Chapter 15

**Blocks** We have covered this subject multiple times, but here is a summary.  

**Block-Level** elements will start on a new line and act as your primary building blocks to shape your page. Ex: h1, p, ul, li.

**Inline elements** the boxes will shape around and between your text. img, b, i. 

Separate your boxes in css using border, margin, padding, background colors, etc. 

**Containing Elements** A block-level element nested inside of another block-level element is known as a parent (containing) element. You can use the div element to separate the child boxes.

**Positioning** In CSS using the _position_ property.

- Normal Flow - Typically if you apply nothing. All of your block-levels will appear on a separate line. They will just drop down vertically one from the next. 

        p {
            positon: static;
        }

- Relative Postioning - This will shift a block-level in relation to where it would be in normal flow. Use position relative, the adjust top, right, bottom, and left. 

        p {
            positon: relative;
            top: 25px;
            left: 75px;
        }

- Absolute Positioning - This takes a block-level element out of the flow and does not impact the postion of the other elements. It is like it isn't on the page. Make sure you apply top, right, bottom, left. Postion things so you don't have overlap.

         h1 {
            positon: absolute;
            top: px;
            eft: px;
            width: ox;
        }
            other elements {
            adjust to not overlap.
            width:
        }

- Fixed Position - keeps an element in the same place even if you scroll. This would me like your main header staying at the top despite where you scroll. 

        h1 {
            positon: fixed;
            width: 100%; 
            set a color, padding, margin
        }

- z-index - use this for overlap. An element with a higher number on the z-index will put the appearance over top of an element with a lower z-index value. 

        h1 {
            z-index: 8;
            this one is on top
        }

        p{
            z-index: 3;
            this is underneath
        }

- float - This will help you to move a block left or right. If you want text to float around an image, this is what you will use. To float multiple boxes side by side, you will want to use your width property in css. 

- clearing floats





**Functions**
Functions allow you to merge a collection or series of statements to perform a task. Functions make code reusable, they help avoid repeat code, allow us to define the code once then run it whenever we need it, and it allows your code to appear a lot cleaner. 

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
3. The curly brackets contain your statement. This will perform your task. This will write it on your webpage.
4. Using the function name in your html code is how you are able to call the function.

### The steps of calling a function.
pg 91 diagram

1. Function stores the steps of a task.
2. You then call the function when you require the script to execute your task. 
3. The function will then perform the code written inside the curly brackets and put it on the website.
4. When it completes the task, the code will continue to run from where you called it.

**Sometimes your functions can seemingly be out of order and they might not work. (Example, you want the userName before the userName was declared.) This doesn't matter if the functions are all in the same script since the computer will run through the entire script before executing the statements.**

### Arguments

-**Arguments** are the values (parameters) held inside the the () of a function name. They can be presented as variables or values.

1. As a Value. (Ex below, 5 is width, 6 is height.)
            
            -getArea(5, 6); 

2. As a Variable. 

        doorWidth = 11;
        doorHeight = 17;
        getArea(doorWidth, doorHeight);

**Review page 95 it JS Duckett.**


**Function Declaration** This creates a function and can be called later. The interpreter looks for variables and functions before it does anything else.

        getArea(width, height) {

        }

**Function expression**  The  intrepreter will interpret a function placed where it expects to see an expression as an expression. An example of this would be stored in a variable.In this format, the intpreter will not find this function before it runs all the lines of code. This is a big difference between this and function declaration.

        let area = getArea(width, height) {

        }

**Immediately Invoked Function Expressions** or IIFE "iffy". These have no name, but they run when the interpreter hits them. If you place this unnamed function where you normally place the value of a variable, that particular variable will hold the value that has been returned by the function. This method is good for when a function only needs to be called a single time. This will help prevent potential conflicts in your code.

**Variable Scope** 

- Local Variables are variables placed inside of the functions code block and can only be used by that particular function. The interpreter creates the variable and then immediately forgets it once the function task is complete. Pop-up windows? login info?

- Global variables are variables that can be used anywhere is your js script. These variables will be stored in the web browser as long as the particular web page stays loaded. Once the webpage is closed, it will forget any and all information. Wide use of these can create conflicting variables, so use these wisely and/or use locals. Globals use more memory than locals. 

An abundance of globals will cause your page to run slower. Locals will help it run faster. Variables outside of a function, global, will conflict if they have the same name.







[Back to code 201 Table](code201Table.md)

[Back to Homepage](README.md)