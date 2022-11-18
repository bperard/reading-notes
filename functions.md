# Functions
In JavaScript, **functions** help save us time by allowing us to put our code into a set order of operations, and save it to be used again, rather than having to write out each step of the function each time we need them in our files.

## Function Syntax
```
function name(parameter1, ... , parameterN) {
    // code
}

name  // reference to function name

name(args) // invoking function name
```
The **function** keyword allows us to declare a new function. We provide this declaration a **name** to be used when referencing or invoking the function we declared. We follow the name with **( )** that contain any **parameters** needed by our function; when our function is invoked, arguments that fit these parameters will be provided to our function to allow it to run. Finally, our declaration has the **{ }** with the code for the function inside of it.

## Invoking Functions
Now that you've made a function, you're going to want to use it in your site. The name of the function is what you'll use for this step, and it's good practice to use a name that provides clarity for the use of the function. In order to **invoke** or execute your function, write the name, followed by ( put needed arguments here ); this will run the function with the provided arguments. If you forget the ( ), you will instead get the function definition, rather than invoking it.
