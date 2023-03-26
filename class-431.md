# 431

## Choosing the State Structure

- Summarize the five principles for structuring state.  
Group related state, avoid contradictions in state, avoid redundant state, avoid duplication in state, and avoid deeply nested state.

## Passing State Deeply with Context

- What problem do Contexts aim to solve?  
Context lets the parent component make some information available to any component in the tree below it—no matter how deep—without passing it explicitly through props.

- What is one technique to try before useContext?  
Passing props

- What hook complements useContext for complex applications?  
useReducer
