# JavaScript Promises?

When we use multiple nested callback functions a big problem arises which is known as Callback Hell or pyramid of doom. The promise is used to handle multiple asynchronous functions and their errors (if occur).

A promise contains two parameters, the first parameter is the function for resolved result and the second parameter contains the function if the result contains an error. Promises are the better choice for handling multiple asynchronous functions than callback functions because it makes code clean and readable.

A promise can be created using a promise constructor as shown below

```javascript
let promise = new Promise(function(resolve, reject){
     //Code for execution
});
```

## Every promise has two properties i.e. state and result.

### State

The state at the start and during the execution of the code is <mark>pending</mark>.

It becomes <mark>fulfilled</mark> when the code executes successfully and a value is returned.

The promise has a <mark>rejected</mark> state when the code executes and any error occurs.

Therefore a promise can have any of the three i.e. pending, fulfilled or rejected at a time.

### Result

Whenever a promise gets out from the pending state to the fulfilled or rejected state it gives a result. A result may be resolved or rejected.

When no error occurs the resolve function executes and whenever an error occurs the reject function executes.

### Consumers

There are two consumers for promises i.e. then or catch. The consumers come into play when the state of the promise resolves or rejects. We pass a function within then and catch consumers. The function within `.then` executes when the promise resolves and the function within `.catch` executes when the promise gets rejected.

```javascript
let promise = new Promise(function(resolve, reject) {
  // Code to be executed which can produce either resolved value or error...
  resolve(value); // when successful completion of code
  reject(error);  // when error occurs
});

// "Consuming Code" (Must wait for a fulfilled Promise)
promise.then( // .then() is a code consumer when no error occurs
  function(value)
);

promise.catch( // .catch() is also a code consumer when any error occurs
  function(error
);
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672221195725/908debca-8e7d-4912-8af9-1dcda7a0d465.png align="center")