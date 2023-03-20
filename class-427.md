# 427

## Thinking in React

- Summarize the five steps of thinking in react.  
1: Break the UI into a component hierarchy
2: Build a static version in React
3: Find the minimal but complete representation of UI state
4: Identify where your state should live
5: Add inverse data flow

## State: A Component’s Memory

- What is one reason a local variable isn’t sufficient for managing a React component?  
Local variables don’t persist between renders.

- What is the argument to the useState hook, and what are the two parts of its return array?  
Argument is initial state; state variable retains data between renders, and a state setter function to update the variable and trigger render.

- How can Component A access state from Component B?  
Move state to their parent component and use props to share setter functions and state references.
