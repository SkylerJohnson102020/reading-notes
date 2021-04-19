# Node.JS

https://www.sitepoint.com/an-introduction-to-node-js/

- Node.JS uses Google's V8 JS engine plus libuv library and is non-blocking, event-based, and an asynchronous I/O blocking. This is Stack Overflow's definition of Node.JS.

- Google Chrome's V8 JS Engine is what Node is built upon - V8 engine is open-source. It's the JS engine that runs in Chrome. V8's features include an http library, a file system API, and other operating system utility methods.

- npm is JS's package manager. npm is a software registry. Access to millions of JS code packages. When downloaded, it will create a package.json file.

- node_modules - npm saves your lodash and libraries that lodash depends upon. lodash is a dependency. lodash is a JS library that gives the user utility functions for typical programming needs using functional programming.

- Node.js is used to automate the dev process of newer, modern JS. Node gives you a lot of building tools.

- Very important to know when using React.

- Running JS on servers is one of Node.js's biggest uses. 

- Node.js execution model - when you connect to a server, a new thread is created to take your request. If you have other operations, it will block the execution meaning the server waits on that until the operation is complete. If new requests come in while dealing with the first, new threads are created. This idea can quickly overwhelm a server and the solution is to typically use more servers.**Node.js on the other hand** is single-threaded and event driven. Everything happens in reaction to an event. Instead of waiting for something to complete, node.js will create a callback and work on the orginal request. Node uses libuv to use the async nehavior. In other words, non-blocking.

- A function is created to make server requests. The function is called each time a new connection is made to the server. An anonymous func. takes 2 args: request and response.

- Node is good for apps that have real time interaction, like chat sites. 

- Node.js speed and scalability are two of it's advantages. Another is using JS on the web server and browser so you don't have to switch back and forth. You can complete everything in one language. Another is JSON, which is the way data is exchanged on the web.

- Other uses, scripting language to automate task that have many errors on your local, write your own command line tool, building cross-platform applications, and create robots.


# Pair Programming

https://www.codefellows.org/blog/6-reasons-for-pair-programming/

### Four foundational skills to learning a language

1. Listening
2. Speaking
3. Reading
4. Writing 

### The 6 reasons for pair-programming

1. Greater Effiency
2. Engaged Collaboration
3. Learning from your colleagues
4. Social Skills
5. Interview preparedness
6. Wor environment preparedness
