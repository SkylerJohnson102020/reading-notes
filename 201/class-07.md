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

[code201Table](201/code201Table.md)

[Back to Homepage](README.md)