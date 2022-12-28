# JavaScript Callback's?

## What is a callback function?

A callback is a function that is passed as an argument to another function. This method is used to execute a function(passed as an argument) when the function has finished.

The JavaScript code executes synchronously according to the calling of the function.

```javascript
function Hello() {
    console.log("Hello");
  }
  
  function World() {
    console.log("World");
  }
  
  Hello();
  World();
```

#### Output

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672133792212/6f65780e-b34c-4fae-9694-2946877b4255.jpeg align="center")

If we reverse the order of calling the function

```javascript
function Hello() {
    console.log("Hello");
  }
  
  function World() {
    console.log("World");
  }
  
  World();
  Hello();
```

#### Output

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672133987062/8a4b94d7-4bfd-4673-b2ba-8ed5276f7684.jpeg align="center")

From the above example, we can understand the working of JavaScript according to the calling of the function.

Let's take another example of subtraction and display its result by using another function.

```javascript
function subtraction(num1, num2, callback){
    let result = num1 - num2;
    callback(result);    
// callback function is called when subtraction function ends execution
}

function showResult(result) {
    console.log(result);
}
subtraction(10, 6, showResult);    // 4
```

The main use of callback function is within the asynchronous function for error handling. *Asynchronous* functions allow multiple things to happen at the same time. setTimeout() is an example of asynchronous function.

```javascript
console.log("Before setTimeout");

setTimeout(() => {
    console.log("Inside the setTimeout function")
}, 2000);

console.log("After setTimeout");
```

#### Output

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672136692432/057b84b7-c7c0-437a-a97b-91988110c1ed.jpeg align="center")

In the output, we see that the function within the setTimeout() executes after 3 seconds after the execution of others.

In the real world, we pass two arguments in the callback function. The first argument is the error and the second argument is the value that we want to pass if no error occurs. The basic work of the callback function as its names suggest is to execute the code after the function completes.