# 438

## async actions

- Why use Redux middleware?  
Enable writing logic that has side effects.

- Consider the Redux Async Data Flow Diagram. Describe the flow in your own words.  
A dispatched action can be handled by middleware to handle, and then the middleware can dispatch a real action object afterward.

- How are we accommodating async in our Redux app?  
Redux Thunk middleware

## thunk middleware

- Why would you need redux-thunk middleware?  
It allows writing functions with logic inside that can interact with a Redux store's dispatch and getState methods.

- Redux Thunk middleware allows you to write action creators that return a ____ instead of an action.  
function

- Describe how any return value from the inner thunk function will be made available.  
Any return value from the inner function will be available as the return value of dispatch itself.
