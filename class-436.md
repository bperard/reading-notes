# 436

## Dan Abramov Redux Tutorials

- What is the first principle of Redux?  
The first principle of Redux is that the entire application state is stored in a single, immutable state tree. This means that the state of your entire application is represented as a single object, which cannot be changed directly. Instead, any changes to the state must be made by dispatching an action, which is a plain JavaScript object that describes the type of the action being performed and any additional data required to perform it.

- What is a store and what do we use our reducers for within that store?  
A store is an object that holds the application state and provides a few helper methods to access the state, dispatch actions, and subscribe to changes. Reducers are functions that specify how the application's state should change in response to actions that are dispatched to the store. They take the current state and an action as arguments, and return the new state.

- Name three Redux store methods given to us by createStore and describe their use.  
getState(): This method returns the current state of the Redux store.

dispatch(action): This method is used to dispatch an action to the Redux store. When an action is dispatched, the store will call the appropriate reducer and update its state accordingly.

subscribe(listener): This method is used to subscribe a listener function to changes in the Redux store. Whenever the store's state changes, the listener function will be called.

- Explain to a non-technical recruiter what combineReducers() does and why it is useful.  
combineReducers() is a helper function that allows you to combine multiple reducers into a single reducer function. This is useful because it allows you to split your reducers into smaller, more manageable pieces, while still maintaining a single, centralized store for your application's state.
