# Understanding the Problem Domain

The problem domain refers to any and all information that defines a problem to which the solution is part of that problem. Like trying to throw darts in the dark, you may not know where to throw and it could be dangerous where the dart lands. The best way to tackle a problem is to break it down into small piece to tackle first gather than easily getting overwhelemed by everything you have to do. 

An Agile project is one where you work in a team tackling task that you are assigned. Now you can still struggle to know what to do since your piece of the pie could still be overwheleming. Best to try to break it aprat and try to understand as much of your problem as possible before starting. Better to do it right the first time than do it all over again.

# Chapter 3 Duckett Object Literals

To quote Duckett John from _Javascript and JQuery: interactive front-end developement_:Indianapolis, IN, John Wiley and Sons Inc., 2014

>"Objects group together a set of variables and functions to create a model of something you would recognize from the real world. In an object, variables and functions take on new names" 

A property is a ariable that is part of an object. For functions that are part of an object, this is known as a method. A property can be a string, number, array, or Boolean. Methods are only functions. Keys represent certain properties within the object.

In an object, you declare it like you would a normal variable in JS only you do = the {}. Within the {} you place all of your properties and methods in these curly braces. Set values with : and separate items with a comma. Name, rooms, and booked are all examples of keys. The object is hotel. **This is literal notation.**

    let hotel = {
        name: 'Indigo',
        rooms: 65,
        booked: 37,

        checkRoomAvailabilty: function() {
            return value.rooms - value.booked;
        }
    };

- **Dot notation** - accessing of properties and methods using the . or also []. To access information about the hotel name:

    let hotelName = hotel.name; 
    let roomsAvailable = hotel.checkRoomAvailabilty();

Above, the vaiable hotelName access the object, hotel, then the member operator (.), then the property "name". Same thing with the second variable only it is accessing the method. You can also use square brackets:

    let hotelName = hotel['name']; 
    let roomsAvailable = hotel['checkRoomAvailabilty']();

The brackets are a good for when property or method name contains a -, is a number, or the variable is used as the property name.

You could essentially use the same notation for multiple listings. Say we have a hotel website that represents numerous hotels where you can book a room. The literal notation above could use the same exact code, the value of the three properties would be the only this changing in our code.

# Chapter 5 Document Object Model

- **DOM** Document Object Model. Operates on it;s own set of rules. These rules are run by the browser and do two things: 1. Make a model of an HTML page. 2. Access then change an HTML page.

The DOM follows the structure of a website using a DOM tree.

- **API** - Application Programming Interface. This allows programs to talk to one another. 

### Four different nodes

- Document - this node represents the entire page and is at the very top of our DOM tree.

- Element - through the document node, you can then access the html elements.This is the first thing to look for once accessing the document. 

- Attribute - these are considered part of the element they are attached to. These aren't children.

- Text - this node is accessible after accessing the element. Cannot have children

- Working with the DOM tree: 2 steps

    1. Find node that represents the element you want.
    2. Use the text, children, and attributes contained within. 

- DOM manipulation - some methods (functions) allow you to add, remove, or create nodes in a tree.

- DOM queries - methods which find elements in tree.

- Caching - the method stores the location of an element so it does not have to find it again, saving time. You can use a variable to store the location, this is not storing the enitre element, but the variable is a reference to where it is in the DOM tree.

- Nodelist - when a method locates more than one node. Each node then is given an index number just like in an array. The order of the items in the nodelist are stored in the same order as on the html page. These look like arrays but they actually aren't, they are **collections**.

- live nodelist - the script updates the page, the list is also updated.

- static nodelist - does not update when script updates the page.

- Two ways to access an item on a nodelist: item() and array syntax.

- item() method - You use this to look at all the info gathered by the selector. 'getElementByClassName('cold'). You then test how many items are in the index using the length propety in an if statment. 

        if (elements.lenth >= 1 {
            let firstItem = elements.item(0)
        })

- array syntax - is preferred method when searching using selectors. This supplies each item if found with an index number and can be accessed using that number. 

- Searching by CSS selector - querySelector() will select only the first match found and querySelectorAll() will create a nodelist of all of them. Searching my css selectors offers greater flexibilty for searching. 

- Repeating actions for the entire nodelist - this requires the use of the for loop using array syntax. The number of items in the nodelist dictates how many times the for loop is run using the .length property applied to the created variable withing the {} of the for loop. Each item is given an array [i] number, as always, starting with 0. You can then change the value of the class att. within thefor loop using the [i] to indicate which one.

    - warmObjects[i].className = 'cold';

The code above applied within the for loop will change the class name and have different css styling applied to it to contain different colors, etc.

- Traversing the DOM - parentNode, previousSibling, nextSibling, firstChild, lastChild.

- Whitespace between nodes can be recognized as text nodes. These make your code easier to read but removing them helps your page run faster. 

-jQuery - Helps browsers be less inconsistent. 

- nodeValue - selects the text of an element. this applies to the method using the properties traversing the DOM. You can use this to update content of a text node.

-textContent - property lets you gather and change of text in containing element and children.

- innerText - you can use this property, but FireFox doesn't support it, CSS issues, and is just slower than textContent.

### Two way to add or remove content from tree: innerHTML & DOM manipulation.

- Adding elements using DOM Manipulation

    1. creatElement()
    2. createTextNode()
    3. appendChild()

- removeChild() - to remove items in tree


### Three ways to add HTML to a webpage:

    1. document.write() (not widely used at all)
    2. element.innerHTML quick and easy changes but brings security risks
    3. DOM Manipulation cleaner and more efficient, takes longer.

- XSS attacks using innerHTML

- Only add content from untrusted sources in the form of text, not as html code. This can cause a breach and websites can be stolen or information can be compromised.

- escaping user content

- attribute nodes - 

- the appendChild() will add new elements to the DOM tree and it will add it at the end of the nodelist. One parameter, adds content to DOM. 

- insertBefore() - use this to add items to the beginning of a nodelist. 

[code201Table](code201Table.md)

[Back to Homepage](README.md)