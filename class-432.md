# 432

## Scaling Up with Reducer and Context

- How do useReducer and useContext work together to simplify state management in a React application?  
useContext cleans up state managment by allowing a parent to provide data to all child components without having to pass props down. In a small component, this may not be a big change, but once you have multiple components that all need the same state, along with multiple components between the parent and relevant child components, this can lead to a lot of prop-drilling pretty quickly. useContext simplifies this by allowing these child components to access this data directly.
useReducer allows us to take complicated state management and condense it into a reducer function. Not only does this allow us to streamline these state transitions into specific dispatches we can view within the same reducer function, this simplifies our event handlers on the pages they're used.
When combined, we can pair useReducer and useContext to remove complicated state management and sharing into their own components, and share our state and dispatch functions directly to the needed components.
