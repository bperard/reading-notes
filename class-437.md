# 437

## Multiple Reducers Example

- Why create multiple reducers?  
Allows us to break complex state management into smaller pieces.

- How would you combine multiple reducers?  
combindeReducers

- How will you manage state as an immutable object? why?  
You create a new state object every time a change is made, this allows you to "time travel" through your state to see how it changed with interactions.

## Redux Docs: Using Combined Reducers

- combineReducers is a utility function to simplify the most common use case when writing ___ _____ .  
Redux reducers

- Explain how combineReducers assembles the new state tree.  
combineReducers will call each slice reducer with its current slice of state and the current action, giving the slice reducer a chance to respond and update its slice of state if needed.

- How would you define initial state in an app using combineReducers?  
createStore function can take preloadedState as its second argument.

## Redux Docs: Combined Reducer Syntax

- Why will you want to split your reducing functions as your app becomes more complex?  
It makes state management more manageable

- The _____ helper function turns an object whose values are different reducing functions into a single reducing function you can pass to ____.  
combineReducers, createStore

- What is a popular convention when naming reducers?  
A popular convention is to name reducers after the state slices they manage.
