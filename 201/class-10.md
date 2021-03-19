# Chapter 10 JS, Error Handling and debugging

Order of execution is helpful when trying to find the source of a problem or just siply knowing how your code is operating. 


Execution contexts - A script will find itself in one of these three contexts: Global, Function, Eval.

The Stack - JS will stack a pile of things to do, meaning, if a statement needs something from another function, it will stack it on top of the current task. Once the new task is complete, it will go back to the original. Every time a new task is added it creates a brand new execution context. 

There are 2 phases of activity everytime the script goes into an execution context that is new. It **prepares** a new scope along with variables, functions, and arguements, then it will **execute** these.

Each execution has it's own variables object. This will contain all the info for the variables, parameters and functions for that particular context.

Lexical scope - an element has access to it's parent element's variables. SO the scope for each execution context is the current element's variable plus each of the parent's.

Inner objects (child) can get outer objects (parent) but not vice versa.

Seven different types of errors: error, syntax, reference, type, range, URI, and eval.

console.group(); You can group console messages together.

        console.group('Area total');
        contain console.info
        and logs.
        console.groupEnd();

console.table(); this will show you a table of objects and/or arrays containing other arrays or objects.

console.assert();checks if a condition is met. If not, it will return a message of false.

Use breakpoints - pausing the execution of a script. You can check on your values stored in variables. pg. 476. Set them up, run the script, and it will stop where you indicated. You can hover over any variable and see the variable value in the JS interpreter's run of the script.

Conditional breakpoints - set up the breakpoint like before and the script will stop at this point only if the condition is true. 

debugger keyword - You can place this keyword in your code to create a breakpoint. You can also use it in a conditional statement and it will, of course, trigger the breakpoint if the condition results true.

Try, catch, finally - **review** 480, 481, 

You can use your own error message. 

        throw new Error('message here');


[code201Table](201/code201Table.md)

[Back to Homepage](README.md)