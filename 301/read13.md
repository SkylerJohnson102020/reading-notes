# CRUD

https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/

- **CRUD - Create Read Update Delete**

#### Methods for CRUD

- Create - use POST
- Read - use GET
- Update - use PUT or PATCH
- Delete - use DELETE

- Status code - first number is the status class, then a code afterward. A reason for the error might be shown as well.

- 100-199 - This refers to the header being received from the client by the server and the server will begin to work through the request. The server will tell the client whether it passed or failed.

- 200-299 - Success, request received. 

- 300-399 - Redirection. Resource unavailable or not at expected location. 
- 400-499 - Error. Invalid request from client to server. (timeouts, missing information, etc)

- 500-599 - Server Error - Commonly referring to overloaded and/or servers not reachable. Sometimes from a client request.

- The 202 code specifically does not necessarily mean success, just that the requirements have been met from an asynchronous request.

- 308 - Permanent Redirect - States that there has been a permanent redirect, change to the location. Resource has been moved to the url stated in location header.

- 204 - No Content - Updates returning no content beck to the client that requested the data.

- 410 - Gone - This resource used to exist but is now gone. The implication is that the server knows that it used to exist.

- 403 - Forbidden - Server understood but denied (did not authorize) the request.

# Video 

https://www.youtube.com/watch?v=fgTGADljAeg

- Why do we need to pull our MongoDB database string out of our server and put it into our .env? 
    We want to put something there that is not localhost and to protect our information.

- What is middleware? 
    Code that runs but before it gets to your routes.

- What does app.use(express.json()) do?
    Allows the server to accept json as a body inside an http method element.

- What does the /:id mean in a route?
    The : in front of id means that it is a parameter. Gives access to whatever the user passes in.

- What is the difference beween PUT and PATCH?
    - PUT to replace something
    - PATCH to update only the information that needs updating, not complete replacement.

- How do you make a defalut value in a schema?
    - You set it inside the Schema object as a key value pair with the key most likely being default:. In the example used in the video, it was default: Date.now.

- What does a 500 error status code mean? 
    Internal server error. Generic error, but indicates that there is a problem with the server.

- What is the difference between a status 200 and a status 201?
    200 - request received and is processing. 
    201 - request received, was successful, and has result of created resource.

[code301 Reading Notes](/301/code301Table.md)