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
