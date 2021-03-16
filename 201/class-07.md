# Domain Modeling

A **constructor function** is one that creates a scenrio of a class that is an object. Defined by function expression, items, parameters, in (). When the function is called, the data from the parameter are then stored in the variables that are created. 

Object-oriented programming:

    1. Keyword instantiates object.
    2. Constructor function initializes the contained properties the object using the variable that was created for the value it is holding.
    3. It is then stored in the object and will be used later.

Generate Random Numbers:
function (min, max) {
    Math.floor(Math.random() * (max - min + 1)) + min;
}

The prototype - You can substitute this in to do the work. So, a variable, EpicCatMovie, can have a prototype, a stand in, and be added methods. Usually a variable will run through a method first before running through the protype, slowing down the speed. It takes longer for it to locate the method when it has to then go through and locate it in the prototype. Using a prototype is good practice since two variables share code, this means less memory consumption.

generate random below is condsidered a method,

EpicCatMovie.prototype.generateRandom = function(min, max)

# Chapter 6: Tables 

Table - content or info in grid format. Use the "table' element. Contents written out one row at a time. Thr tr tag is used to indicate the start of each row. The td tag is used to represent a cell. The th tag is used to label the heading or row.

colspan attribute lets you label how many cells across an element wil take. colspan = "2" will cover two spacescolumns across.

rowspan attribute lets you cover cells going down. rowspan = "2" will cover two cells vertically. 

Long Tables are a bit different. Set your tr headings contained in the "thead" element.The body of your table will sit in the "tbody" element. "tfoot" for the footer of the table. 


## Chapter 3 Functions, Methods, and Objects

 - Constructor Function - Rather than just write out every single object in object literal notation, which can use a ton of code, you use this constructor function. You create a template for the object, give it place holders with "this.", and pass the information from the variable below. The constructor function is capitalize to remind you that you need to use the new keyword when wanting to pass a new object through the constructor function. so:

        function Hotel (name, rooms, roomsBooked) {
            this.name = name;
            this.rooms = rooms;
            this.roomsBooked = roomsBooked;
            this.checkAvailabiltity = function (){
                return this.rooms - this.roomsBooked;
            };
        };

        let hotel1 = new Hotel(Indigo, 56, 23);
        let hotel2 = new Hotel(Radisson, 100, 72);
        let hotel3 = new Hotel(Blue, 75, 50);

        The += operator - You want to use this when you are adding content to a already used variable.  

An array is a unique kind of object. It stills holds the key/value pairs but the key is going to be an index number, not the property name.


Built in objects are objects like a browser window and/or webpage shown. These are objects that make up the basic tools for pages. 

Object Model - a collection of objects that together they represent a model of something much bigger.

Three different kinds of built-in models:
    1. Browser Object Model
    2. Document Object Model
    3. Global JS Objects

Six types of data in JS: String, number, boolean, null, undefined, and object (arrays are objects). Functions are technically alos objects.

### Review
**Three built-in models**
**Working with decimals (pg. 133)**
**Math object (page 134)**
**Date and Time (pg. 136-137, 139)**

The order and syntax for date and time:

year 4 digits
month 0-11
day 1-31
hour 0-23
minutes 0-59
seconds 0-59
milliseconds 0-999

Computers will return date and time in milliseconds, use your math object and floor to get a readable figure.



[code201Table](201/code201Table.md)

[Back to Homepage](README.md)