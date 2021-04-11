# React

- Immutability - this makes it easier on us. An object or value that is immutable can't be changed. Each updates creates a new value and leaves the old one alone. Once the element is created, the children or atts cannot be changed.

- props - properties. Is passed as an object. Use props when passing state from parent component to child.

- components - This is what React is built upon. These are it's building blocks. These are simply either a JS class or function that takes in props then returns a React element and describes how a section will appear on the UI.

- Function components - these are literally JS functions.Takes in an argument and returns a React element. Use class in this same way.

- concat() - not like the array push(). This method does not change the original array.

- map() - it's use is to map data to other data coming in from arrays. We can use this to map our history.

- key - Term only in React. Takes in list items and re-renders by searching for keys. If the new/ current list has a new key, React creates a component. If the key is not found on the new list from the previous list, that component is detroyed. If our keys match, component is moved. If changed, the component is destroyed and re-created with a new state.

# JSX 

https://reactjs.org/docs/introducing-jsx.html

- JSX is a syntax extension of JS. An example looks like:

        const element = <h1>Hello!!!</h1>;

Any valid JS expression can go inside curly braces.

JSX IS also an expression. Meaning you can use JSX in if statements and for loops. You can give it variables, take in arguments, and return it from your functions.

Use quotes to specify your string literals as atts. Use quotes for string values, curly braces for expressions, not both in same att.

ReactDOM uses camelCase.

Children in JSX. These looks like html tags and these tags can have children. Example:

        const element = (
            <div>
                <h1>Bonjour!</h1>
                <h2>Great that you are here!</h2>
            </div>
        );

JSX prevents "injection" attacks. You are safe to put user input in JSX since React DOM will escape values before rendering them using JSX. Basically, this prevents you from putting any content or anything that is not written in your app.Everything here converts to a string before rendering. This will prevent cross site scripting attacks.

React.createElement() creates a objects and runs some checks helping your code to be more bug free.

# Rendering Elements

https://reactjs.org/docs/rendering-elements.html

React elements are simple objects and are easy to create. React DOM updates the DOM and matches React elements.

Rendering - ReactDOM.render():
Apps built with React only may have only one root DOM node, like a div. If you are working on a pre-existing app, you can have many isolated root DOM nodes.

A React element is it's own point in time, immutable.

React will only update what it deems necessary. Rather than updating the entire app, the ReactDOM compares an element plus it's children to the previous and will only update where necessary to get the DOM to the state wanted.

# Components and Props

https://reactjs.org/docs/components-and-props.html

Components are individual pieces of the puzzle, and they're reusable. Each piece is isolated. Components are like functions on class in JS. They take in props and return React elements describing the appearance of the screen.

We know the ReactDOM tags, but we can make user-defined components. 

        const element = <Hello name="Skyler" />;

React will see an element with this user-defined component format and it passes JSX atts. and children into this user-defined component as one object. This object is props. You can split up a single components into multiple parts for readability. Name component's props from the components point of view, this helps readability.

Components cannot change their props andmust be pure functions. React components have to behave like pure functions regarding their props. State takes care of the changes without violating this rule.

[code301 Reading Notes](/301/code301Table.md)