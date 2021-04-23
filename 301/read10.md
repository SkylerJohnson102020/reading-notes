# Understanding the JS Call Stack

https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/

- Call Stack - it's initial use are function calls. Calls are done from top to bottom, in order one at a time, synchronous. The understanding of this is critical in asynchronous programming. Single-threaded.

- callback function - a function passed into another function as an argument. This callback will be invokde inside of the outer function. The call stack acts upon these callbacks during the execution of the script after the callbacks have been added to the stack by our event loop.

- LIFO - A data structure principle. This is the basic understanding of the call stack. **Last In, First Out.** The last function to go in, the first to come out.

- Manage function calls - one at a time.

- stack overflow - Recursive function, meaning, a function that calls itself but does not have an exiting point. This will throw an error.

        function callMe(){
            callMe();
        }

        callMe();


# JS error messages

https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors

_ **Types of errors**

    1. Reference errors - simple as an undeclared variable. (not defined) 
    2. Syntax errors - invalid object that you are trying to parse in a JSON file. Shifting around commas, adding a curly, removing an extra token, etc.
    3. Range errors - trying to return a negative position in an array will throw this error.
    4. Type errors - data type (string, number, boolean, ...) in not compatible. Like trying to access a property of variable that doesn't exist.
    

- Debugging - use those console.logs! 

- IIFE - Immediately Invoked Function Expression

- Call stack is available in dev tools. Adding names to your functions can help you track the call stack better.

- Handling errors - try/catch. This helps avoid "Uncaught errors". console.error(). try/catch will allow the script to continue to run. This is good to use when your function logic is long.

- Tools for avoiding runtime errors - meaning, only able to see errors once you run it.

        1. Quokka - this analyzes your code as you write.
        2. eslint - cathes errors along the way and marks them.
        3. TypeScript - for a stong typed approach.

[code301 Reading Notes](/301/code301Table.md)