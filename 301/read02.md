# React State and Lifecycle

https://reactjs.org/docs/state-and-lifecycle.html

- State - not quite the same as props, but similar. It is controlled only by that one compononent and is private to that componenet. This is responible alone for changing the state of say the ticking clock.

- In a class constructor, the base constructor needs to always be called using props.

- Mounting - Whenever something is renderered to the DOM (ReactDOM), like our Clock, we need to up the timer when this clock is rendered initially.

- Unmounting - the opposite, clering it out.

- setState - this will set updates to state to the component's local state.

    - You do not want to directly modify state, use setState instead.

    - updates to state can be asynchronous, meaning React can bundle multple calls together regardless of when they are fired.You may want to use a setState method that takes in a function rather than an object.

    - React will merge your state updates

- state can be passed down to children using props.

- data flows down - top down.

# Handling Events

https://reactjs.org/docs/state-and-lifecycle.html

- name React events using camelCase

- pass function as event handler, not string.

# Conditional Rendering 

https://reactjs.org/docs/conditional-rendering.html

- use variables to store elemets for conditionals.

- embed JSX expressions using {}.

- Use your conditional operators in your statements. Using && will create a strict equals to scenraio. If the first condition is false, the second is skipped.

- the ? operator. This is a conitional operator rendering true or false.

- If wanting a component to hide itself and not render it's output, make that component "return null". You can of course skip this using an if statement. Setting the return null in the component will skip it in your render method.

[code301 Reading Notes](/301/code301Table.md)