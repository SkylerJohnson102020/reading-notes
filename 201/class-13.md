# Local Storage

http://diveinto.html5doctor.com/storage.html

Cookies were used early on in web's history to store small amounts of data, however, there are downsides to these:

1. Cookies come each time an HTTP is requested, slowing the down the application while the same data runs and runs.

2. Unencrypted data is sent with every request.

3. They have a limite of 4 KB, but can still slow the app down.

HTML5 storage - A way to store key/value pairs from websites locally with the client browser.

The data still persists like cookies once you leave, close, turn off, etc., the difference is that the data isn't transmitted back to the server.

To check for storage, run the code listed under "check for HTML5 Storage" from the article. 

### Using HTML5
 All data is stored as a string, so in order to change this, you will have to use the parseInt() or parseFloat() to change your data.

The use of getItem() and setItem() methods will be used.

Also, removeItem() or clear() methods.

Each origin gets 5 MB of storage as a default. Remember, you are storing stings.


[code201Table](/201/code201Table.md)

[Back to Homepage](README.md)