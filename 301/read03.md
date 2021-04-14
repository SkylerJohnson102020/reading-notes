# Lifting State Up

https://reactjs.org/docs/lifting-state-up.html

Components need to have the data that is changing be the same. The best way to do this is to lift up state up to the closest parent component.

Lifting state "up" (sharing state) - this is achieved by moving the shared state up the chain to the closest ancestor or parent that the components share that need the shared state.

We generally want one component, typically the parent component, that is the "controller" or the one handlling most of the action. This can provide all the data the other, child, components need. 

State asks React to re-render itself each time.

# Lists and Keys

https://reactjs.org/docs/lists-and-keys.html

map() function to take in an array. map() calls this function once for each item in the array. This loops through the array. Elements that are contained within the map() function call require keys. This is good practice.

Build collections of elements in JSX {}.

Keys - these are important since it helps React be able to identify what items changed, added, or removed. These are useful and should be placed within the context of the array. These need to be uniquely named among other children of the parent (siblings). You cannot pass keys to other components, use props instead when passing something.

Extracting Components using Keys - Keys only really apply to the surrounding context of the array.

# The Spread Operator (...)

https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab

This operator is a quick and easy way to add items to an array, combing arrays/objects, and having it in a function's arguements. The third one would spread an array into the arguements.

The example given in the article shows a Math.max() method being used to check for the largest number number in our array. This returns everything and returns NaN. Using ... will spread the numbers out as separate arguments rather than just one being the array as a whole.

Spread expand objects that are iterable (typically arrays).

Use the spread operator to copy an array, combining arrays, add new array items, concat. arrays, math functions, use array as arguments, adding list item, adding onto to state (React), combining objects, NodeList conversion to array,

(...) is useful when working with objects and arrays.

[code301 Reading Notes](/301/code301Table.md)