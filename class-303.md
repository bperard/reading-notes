# 303

## React Docs - lists and keys

- What does .map() return?
New array

- If I want to loop through an array and display each value in JSX, how do I do that in React?
Put each JSX element in curly braces.

- Each list item needs a unique ____.
Key

- What is the purpose of a key?
Attribute that serves as a unique identifier for React to determine which elements have changed during a render.

## The Spread Operator

- What is the spread operator?
Passes an iterable item as separate arguments.

- List 4 things that the spread operator can do.
Copying an array, concatenating or combining arrays, using Math functions, using an array as arguments

- Give an example of using the spread operator to combine two arrays.
const combinedArray = [...arrayOne, ...arrayTwo]

- Give an example of using the spread operator to add a new item to an array.
const arrayItems = [newItem, ...arrayItems]

- Give an example of using the spread operator to combine two objects into one.
const newObject = {
  ...objectOne,
  ...objectTwo
}

## How to Pass Functions Between Components

- In the video, what is the first step that the developer does to pass functions between components?
Makes the function in the component where state exists.

- In your own words, what does the increment function do?
Maps through an array to find the passed in key, then increments the value.

- How can you pass a method from a parent component into a child component?
Passed as a prop

- How does the child component invoke a method that was passed to it from a parent component?
this.props.methodName
