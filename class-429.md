# 429

## Extracting State Logic into a Reducer

- What is the motivation for adding a reducer?  
Components with many state updates spread across many event handlers can get overwhelming. For these cases, you can consolidate all the state update logic outside your component in a single function, called a reducer.

- What are actions in the context of a reducer? How are they different than setting state directly?  
Managing state with reducers is slightly different from directly setting state. Instead of telling React “what to do” by setting state, you specify “what the user just did” by dispatching “actions” from your event handlers.

- What common list operation is useReduce named for, and why?  
They are actually named after the reduce() operation that you can perform on arrays. React reducers are an example of the same idea: they take the state so far and the action, and return the next state. In this way, they accumulate actions over time into state.

- When should you switch from useState to useReducer?  
Use a reducer if you often encounter bugs due to incorrect state updates in some component, and want to introduce more structure to its code.
