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




[code201Table](code201Table.md)

[Back to Homepage](README.md)