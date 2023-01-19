# 310

## Understanding the JavaScript Call Stack

- What is a ‘call’?  
Function invocation

- How many ‘calls’ can happen at once?  
The call stack is synchronous, one call happens at once.

- What does LIFO mean?  
Last In, First Out; the last function pushed into the stack is the first to be popped out, when the function returns.

- Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.  
![Call Stack](./LIFO%20Call%20Stack.png)

- What causes a Stack Overflow?  
When a recursive function without an exit point is invoked, a stack overflow will occur once the hosting environment maximum call size is exceeded.

## JavaScript error messages

- What is a ‘reference error’?  
Attempting to use a variable that hasn't been declared yet.

- What is a ‘syntax error’?  
This occurs when you have something that can't be parsed in terms of syntax.

- What is a ‘range error’?  
Trying to manipulate an object with some kind of length and giving it an invalid length.

- What is a ‘type error’?  
The types you are trying to use or access are incompatible.

- What is a breakpoint?  
Allows you to stop execution of your code at a specified point and view the output to evaluate what is happening.

- What does the word ‘debugger’ do in your code?  
The debugger statement stops the execution of JavaScript, and calls the debugger.
