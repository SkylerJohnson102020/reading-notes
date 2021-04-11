# React

- Immutability - this makes it easier on us. An object or value that is immutable can't be changed. Each updates creates a new value and leaves the old one alone. 

- props - properties. Use props when passing state from parent component to child.

- components - This is what React is built upon. These are it's building blocks. These are simply either a JS class or function that takes in props then returns a React element and describes how a section will appear on the UI.

- Function components - simpler way to write a component. Only contains render method and doesn't need it's own state. Can take in props and returns what is to be rendered. 

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



[code301 Reading Notes](/301/code301Table.md)