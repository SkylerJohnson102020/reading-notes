# Thinking in React

https://reactjs.org/docs/thinking-in-react.html

- Step 1 - Break UI into a component hierarchy. 
Keep in mind a good top-down flow. Strive to make sure that each component is handling one thing, called the **single responsibility rule**. Follow this principle when you have to create a new object or function/class. (Draw out a flow chart, data model) Remember to break your UI into components and each one will match a piece of your data model.

- Step 2 - Static version build
If you are building a static version of your app, you will not need to use state since state is used for interactivity between the separate components. As always, for passing data from parent to child, use props.

- Step 3 - ID the minimal representation of State in the UI. (Completed State)
State to trigger changes in data, review previous reading assignment for more on state. Go for the minimum use of state needed in order to get the map to operate as desired.

Ask these three questions:
    - Is data being passed from the/a parent through props? (If yes, then most likely not state.)
    
    - Is data staying unchanged? (If yes, then most likely not state.)

    - Are you able to compute the data based upon other props or state in the component? (If yes, then it is not state.)

- Step 4 - ID where you want your state to be.
After you id where you don't need state and just need props, go through and see where you need it. In other words, which components are **mutable.** 

Follow these steps when figuring out where to place state:
    
    - Find each component that renders data based upon that state.

    - Find the top level component. (common ownership)

    - The owner of state should be a top-level component.

    - If there is not a clear place to put it, create a new component where state will live. Make sure this is a top-level component.

Step 5 - Add Inverse data flow
So now we need to update the parent component from the children. Basically, your top-level component will have callbacks to get the data back from it's children.

[code301 Reading Notes](/301/code301Table.md)