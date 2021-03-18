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








[code201Table](201/code201Table.md)

[Back to Homepage](README.md)