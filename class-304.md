# 304

## React Docs - Forms

- What is a ‘Controlled Component’?  
An input form element whose value is controlled by React in this way is called a “controlled component”.

- Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.  
Update the state as they enter it so input and state are always the same, this allows the value to be shared with other elements/components as the user interacts with our site.

- How do we target what the user is entering if we have an event handler on an input field?  
this.state.value

## The Conditional (Ternary) Operator Explained

- Why would we use a ternary operator?  
Shorten a conditional statment into one line of code.

- Rewrite the following statement using a ternary statement:

```JavaScript
if(x===y){
  console.log(true);
} else {
  console.log(false);
}
```

```JavaScript
x === y ? console.log(true) : console.log(false);
```
