# 439

## Redux Toolkit (RTK)

- What concerns are addressed by Redux Toolkit?  
The Redux Toolkit package is intended to be the standard way to write Redux logic. It was originally created to help address three common concerns about Redux:

"Configuring a Redux store is too complicated"
"I have to add a lot of packages to get Redux to do anything useful"
"Redux requires too much boilerplate code"

- What does configureStore() do?  
configureStore(): wraps createStore to provide simplified configuration options and good defaults. It can automatically combine your slice reducers, adds whatever Redux middleware you supply, includes redux-thunk by default, and enables use of the Redux DevTools Extension.

- How would I use createSlice()?  
createSlice(): accepts an object of reducer functions, a slice name, and an initial state value, and automatically generates a slice reducer with corresponding action creators and action types.

## MobX

- What is Mobx?  
MobX is a simple, scalable and battle tested state management solution.  MobX is a standalone library, but most people are using it with React.

- How does MobX make it “impossible” to produce an inconsistent state?  
MobX makes sure that everything that can be derived from the application state, will be derived. Automatically.

- How would we build a reactive user interface?  
The observer HoC wrapper from the mobx-react-lite package fixes that by basically wrapping the React component in autorun. This keeps the component in sync with the state.
