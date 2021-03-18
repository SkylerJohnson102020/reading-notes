# Chapter 7 Forms
 
What is a form control? A form control is a page that collects user data. Something like the main page for Google. These range from inputs like password, entering text for comments, radio buttons, checkboxes, drop-down boxes, submit buttons, image buttons, uploading files, etc.

How do they work? 

    1. The user clicks/types their info, then submits.
    2. Names of all form controls are sent to the server as well as the value entered.
    3. Server processes, and also may store in database.
    4. Server creates a new page to send back to the same user using the information that the server was given.

Information is passed to the server in the form of name/value pairs.

## Structure page 151

The form html element contains the form controls. This element will also require an _action_ attribute and typically a _method_ and _id_ att. as well.

The _action_ att. - The value it holds is the url for the page based in the server that will receive the content input on the form once it is sent.

_method_ -  Your method is responsible for sending the form and this happens in one of two ways: _get_ or _post_. Using the _get_ method, the values from a form are pasted to the end of the url in _action_. Good for short forms and simple data from the server. The _post_ method posts the info to HTTP headers. Use this method if your form:

        1. allows the option to upload files
        2. long in length
        3. sensitve (passwords)
        4. adds or removes info from a database

Input (pg. 152) - used for the creation of many different controls. Use the type="text", name, size, and maxlength(limits characters a user can input) atts.  

Password input - when you enter type="password" as an att. for your input element, it creates a box where the characters are blocked. The name att. is used to identify the name of the pw that was put it, maxlength again. 

textarea element - used to enter input with multiple line of text, like an "add comments" box. You need an open and close tag for this one. Text contained within the tag will appear in our text box once loaded. Use height and width in css to control size.

Radio buttons on pg 155. type="radio" You have to input each button separately using the input element. Give it a value="" to give your button a label so the user knows what they are selecting. checked att is something you use for this.

Checkbox, same idea as radio button. type="checkbox" checked att is something you us here too.

Drop-downs - use select element. This will contain one or more option elements. Use option to specify an option to select. Text between the tag will be shown in the drop down. Value att., the type of data being sent to server. Selected att. this will show/indicate the selected option (highlight or checkmark)

Multiple select box - use select element for this. use the size att. to adjust how many values you want displayed. use the number of options you want to appear. The multipl att. allows user to select more than one answer

File input box - use input element. use this to upload files. specify type="file". This will generate browse and upload buttons. 

Submit button - use input element and set type="submit". the value att. let's you specify what text will show on the button. 

image button - use input element and specify type="image". You can use an image as your button. Follow the code on pg. 161. 

Button and hidden controls - use button element. You can combine text and images within the button container. use input element to use your type="hidden". Review pg. 162.

Labelling form controls. You will want to review this on page 163. 

Fieldset element 

legend element

Form validation - You a user doesn;t input anything and the server return a message saying to the user "fill this out". 

Enter date - use input element and specify type="date"

email - use input and specify type="email". For websites use type="url". 

type="search" for search input.
placeholder - use this to put placeholder text in you bar that will disappear once the use clicks on the bar.

**Follow example on pg 171!**

# Chapter 14 Lists, Tables, and Forms

Bullet point style
list-style-type

    ul - you can use disc, circle, or square
    ol - decimal, decimal-leading zero, lower-alpha, upper-alpha, lower-roman, upper-roman.

    ol {
        list-style-type: decimal-leading-zero;
    }

You can also use images for the bullet points using list-style-image.

        ul {
            list-style-image: url("photos/salmon.png.")
        }
        li {
            margin: 10px 0px 0px 0px;
        }

Positioning text in relation to bullet point. You can set traditional _outside_ where the point is to the left of the text or indented _inside_ where the point becomes part of the text and indents the first line.

        ul.salmon {
            list-style-positon: inside;
            list-style-position: outside;
        }

Shorthand _list-style_

        ul {
            list-style: inside circle;
            width: px;
        }
        li {
            margin: px px px px;
        }

**Table Review (putting it together) pg. 337.**

_empty cells_ - This property can hide empty cells. Use three att.: show, hide, and inherit.

gaps between cells - _border-spacing_, _border-collapse_. 

    td {
        bacground-color:;
        padding: px;
        border:;
    }
    table.1 {
        border-spacing: 5px, 5px;
    }
    table.2 {
        border-collapse: collapse;
        no pace between cells
    }

Styling text inputs **pg. 342**
:focus pseudo class to change background-color of of text-input when used.
:hover pseudo class sets different styles when the cursor is over these.

Styling buttons **pg343** 

Fieldsets and Legends - This is good for longer forms to group all the information together. Set width, color, background-color, border and radius, and padding.

Cursor styles 
        
        a {
            cursor: auto, crosshair, default,
            pointer, move, text, wait, help, or load an image.
        }

**Code example on page 351.**


[code201Table](201/code201Table.md)

[Back to Homepage](README.md)