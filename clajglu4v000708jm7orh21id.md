# Functions in JavaScript

A Function is a set of code put together inside it which when called repeats its computations repeatedly and gives output. 

The idea function is made by putting some task together, so that instead of writing same code again & again for different inputs, we can call the function once. Thus the code repeatation reduces and lines of code reduces. This increases the readability of the code. Hence functions are the basic building blocks of JavaScript.

## Syntax
![Syntax](https://www.tutorialstonight.com/assets/js/javascript-function.webp align="right")

According to the syntax we can define the function for getting square of a number like

```
 function square(a){
    return a*a;
}
let num = square(4);
console.log(num);    //16
```

In the above example we have seen a function for doing square of a number and getting output in the console of the browser.

We can also pass multiple arguments in the function. The values passed in the parenthesis braces `()` are known as arguments and are further used in the code block of the function. 

For multiplication of two number we have to pass two arguments in the function.

```
 function multiply(a,b){
    return a*b;
}
let numbers = multiply(4,3);
console.log(numbers);    //12
``` 

The above code takes two values within the braces as arguments and outputs the multiplication of both arguments in the console of the browser.