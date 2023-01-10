# 302

## React lifecycle

- Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?  
render

- What is the very first thing to happen in the lifecycle of React?  
The constructor for a React component is called

- Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates  
Constructor, render, React Updates, componentWillUnmount

- What does componentDidMount do?  
This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions. If you do that, don’t forget to unsubscribe in componentWillUnmount().

setState() can be called here, but it should be used sparingly, because it will cause a rerender, which can lead to perfomance issues.

## React State Vs Props

- What types of things can you pass in the props?  
Anything we might want to use to initialize a component.

- What is the big difference between props and state?  
Props are passed into a component, state persists within a component.

- When do we re-render our application?  
When the state is changed.

- What are some examples of things that we could store in state?  
Anything that should cause a re-render after something happens, like a dynamic counter or status.
