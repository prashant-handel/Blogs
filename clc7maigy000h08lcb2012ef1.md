# JavaScript Finally Clause?

We use try and catch for error handling in JavaScript. But there is another keyword that is used with try and catch. The keyword is finally. When we write code using try and catch for handling errors. If the code is errorless, then try block statements executes. And if it contains error, then it is passed into the catch statements and executes the catch statement.

If we write finally keyword after try and catch and give some statements withing the finally block, the statement within this block always executes if there is any error or not in the function.

```javascript
try {
    // try_statements
} 
catch(error) {
    // catch_statements  
}
finally() {
    // codes that gets executed anyway
}
```

We can also add finally method with the consumers of the promise method (then and catch). In promise also the finally method always can also executes if there is any error or not in the function.

```javascript
promise
    .then(result => {
        // process the result
    })
    .catch(error => {
        // handle the error
    })
    .finally(() => {
        // clean up the resources
    });
```