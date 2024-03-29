# 305

## React Docs - Thinking in React

- What is the single responsibility principle and how does it apply to components?  
A component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.

- What does it mean to build a ‘static’ version of your application?  
A version with no interactivity that renders the UI and static data how you planned.

- Once you have a static application, what do you need to add?  
Figure out the absolute minimal representation of the state your application needs and compute everything else you need on-demand.

- What are the three questions you can ask to determine if something is state?  

1. Is it passed in from a parent via props? If so, it probably isn’t state.
2. Does it remain unchanged over time? If so, it probably isn’t state.
3. Can you compute it based on any other state or props in your component? If so, it isn’t state.

- How can you identify where state needs to live?  
Identify every component that renders something based on that state.  
Find a common owner component (a single component above all the components that need the state in the hierarchy).  
Either the common owner or another component higher up in the hierarchy should own the state.  
If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

## Higher-Order Functions

- What is a “higher-order function”?  
Functions that operate on other functions, either by taking them as arguments or by returning them.

- Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?  
Returns a function that takes in input m and returns a boolean comparing m > n.

- Explain how either map or reduce operates, with regards to higher-order functions.  
These functions both take in a callback function as an argument.
