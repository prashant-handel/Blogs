# Promise Chaining in JavaScript

Promise chaining is used for handling more than one asynchronous task one after the other.

## What is Promise Chaining?

We use asynchronous functions which return promises and use resolve values with the help of `.then`. And that value we further use in another asynchronous function within another `.then` block and so on. At last, we give `.catch` block for handling errors. If there is any one error in any asynchronous function, it will be handled by the `.catch` block. This method of writing `.then` methods continuously one after another is known as <mark>'promise chaining'.</mark>

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672310338692/010ab20f-e2a0-4b79-ab73-400b6ab8605b.png align="center")

## Syntax

```javascript
new Promise(function(resolve, reject) {

  setTimeout(() => resolve(1), 1000); // This methods gives output after 1 sec
// Passes the resole value i.e. 1 to the .then method
}).then(function(result) { // (**)

  alert(result); // 1
  return result * 2;    // resolved value 2 passes to the next .then

}).then(function(result) { // (***)

  alert(result); // 2
  return result * 2;    // resolved value 4 passes to the next .then

}).then(function(result) {

  alert(result); // 4
  return result * 2;
}).catch(function()=>{
console.log("Some error occurred") // it doesn't call because there is no error
});
```

## How does promise chaining work?

The initial promise resolves in a defined time, then the `.then` handler is called which in turn creates a new promise (resolved with another value). The next `.then` gets the result of the previous one and passes it to the next handler and so on.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672310223771/62e92ad4-3901-4c07-99e6-ff8542e256d0.png align="center")

## Attaching multiple handlers to a promise

We can provide multiple handlers to a promise which handles promise one after the another in a sequence. The handlers will get the value once the promise gets fulfilled. For better understanding lets take an example.

```javascript
let p1 = new Promise((resolve, reject) => {
    // alert("Hey I am not resolved")
    setTimeout(() => {
            resolve(15);
    }, 5000)
})

// This handler will be called first
p1.then((value) => {
    console.log(`first handler with value ${value}`);
})

// This handler will be called second
p1.then((value) => {
    console.log(`second handler with value ${value}`);
})
// This handler will be called third
p1.then((value) => {
    console.log(`thirdhandler with value ${value}`);
})
```

### Output

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672311190034/19b26b41-c554-45cf-949f-ac59b47ece5a.jpeg align="center")