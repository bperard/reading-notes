# 426

## React Quick Start

- What are the building blocks of a React app?  
components

- What is the difference between an HTML element and a React component?  
Components use a capital letter

- What is JSX and why do we use it?  
JSX is stricter than HTML. You have to close tags like <br />. Your component also can’t return multiple JSX tags. You have to wrap them into a shared parent, like a <div>...</div> or an empty <>...</> wrapper.

- Describe the process of embedding JavaScript expressions in JSX.  
Put the JS expressions in {}

- Does React or JSX have any special features for iteration or conditional logic?  
The key attribute is used by React to track when items are added, deleted, and/or updated

- How does React know to respond to a user’s inputs?  
event handlers

- What word indicates that a React component manages data with a Hook?  
use

- How can two react components share data?  
props

## Render and Commit

- What are the three steps of refreshing a React UI?  
Triggering a render, rendering the component, and committing to the DOM.

- How do you trigger updates to a component after the initial render?  
The component’s (or one of its ancestors’) state has been updated.

- Does React recreate DOM nodes on every rerender?  
No, React only changes the DOM nodes if there’s a difference between renders.

- After React has updated the DOM, what still needs to happen before the user sees the change?  
After rendering is done and React updated the DOM, the browser will repaint the screen. Although this process is known as “browser rendering”, we’ll refer to it as “painting” to avoid confusion throughout the docs.
