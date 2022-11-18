# Loops
One of the benefits of using functions is to not have to rewrite code we've already used. However, as you start to code, you may realize that you're having to use the same functions multiple times in a row to accomplish a task. To solve this problem, we can use **loops** which allow us to set conditions on how our functions operate.

## For Loop
```
for (let initialValue = 0; initialValue < limitValue; initialValue + loopIncrementValue) {
    // code goes here
}
```
The code block above contains a **for loop**, which sets the conditions for how many times the code contained within the **{ }** runs. The *initialValue* of the loop sets the value of the **iterator**; this doesn't have to start at 0, the proper value will be determined by what you'd like to accomplish. The next portion sets some type of condition that will leave the for loop when met; in this example, the loop ends when the iterator is no longer less than the *limitValue*. In the final piece of our loop, we determine what happens to our iterator after each loop; in the above example, a *loopIncrementValue* is added each loop until the condition is met to end the loop.
