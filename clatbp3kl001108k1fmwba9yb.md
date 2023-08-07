---
title: "Variables in JavaScript"
datePublished: Wed Nov 23 2022 07:27:15 GMT+0000 (Coordinated Universal Time)
cuid: clatbp3kl001108k1fmwba9yb
slug: variables-in-javascript
cover: https://cdn.hashnode.com/res/hashnode/image/unsplash/PsRUMc7vilg/upload/v1669188381862/e5ZyOvejn.jpeg
tags: variables, javascript, variable-declaration, variables-and-constants, types-of-variables

---

JavaScript variables are used to store various types of data and do computations using that variables. In simple language variables are containers for storing data values. Similarly like we store different types of items in different containers in our kitchen.

## There are mainly three ways to make variables in JavaScript

### 1\. var method

The `var` method is used for creating variables in JavaScript which are either local or global in scope. It is the previously used method for declaring variables in JavaScript.

```javascript
var a = 53;    // contains integer type of data
var b = "Aditya"    // contains string type of data
var c = {name: "John", RollNo: "123"}    // contains object
```

### 2\. let method

The `let` keyword is introduced in ES6 and is used to create block-scoped variables. This is the latest method for declaring variables in JavaScript.

```javascript
let a = 53;    // contains integer type of data
let b = "Aditya"    // contains string type of data
let c = {name: "John", RollNo: "123"}    // contains object
```

### 3\. const method

The `const` method is used for creating variables in JavaScript which we never want to change. This means that once a constant has been declared, its value cannot be changed.

```javascript
const a = 10;
console.log(a);    // 10

a = 15;    // Uncaught TypeError: Assignment to constant variable.
```

## Now the basic question arises. What is the difference between `var` and `let` keyword in JavaScript.

The basic differences are as follows-

#### The main difference between `let` and `var` is that scope of a variable defined with let is limited to the block in which it is declared while variable declared with `var` has the global scope. So we can say that `var` is a keyword which defines a variable globally.

```javascript
function greaterValue() {
    var a = 5;
    if (a > 2){
        var b = 2;
        console.log(`${a} is greater than ${b}`);
    }
    console.log(a);
    console.log(b);
}
greaterValue();
```

Output- `5 is greater than 2 5 2`

By using `var` for declaring `a` we can access `a` anywhere within the function and `b` is also accessible within the block of the function. `b` is defined within the if block but within whole funciton greaterValue().

If we try to declare above variables using let at the place of var, then-

```javascript
function greaterValue() {
    let a = 5;
    if (a > 2){
        let b = 2;
        console.log(`${a} is greater than ${b}`);
    }
    console.log(a);
    console.log(b); // gives error
}
greaterValue();
```

Output- `5 is greater than 2 5 Uncaught ReferenceError: b is not defined`

The above code will give error as shown in the output. The Uncaught ReferenceError will be displayed because we try to access the variable `b` outside the if block which is not possible when we are using `let` keyword for declaring the variable.

#### A variable declared with `var` can be redeclared again.

```javascript
var a = 5;    // 5
var a = 1;    // 1
```

#### A variable declared with `let` cannnot be redeclared again.

```javascript
let a = 5;    // 5
let a = 1;    // Uncaught SyntaxError: Identifier 'a' has already been declared
```

#### Redeclaring a variable with `var` in a different scope or block changes the value of the outer variable too. like-

```javascript
var a = 5;
console.log(a); // 5
{
    var a = 1;
    console.log(a); // 1
}
console.log(a); // 1
```

In the above example we have changed the value of `a` within block inside the block where a was declared. This will change the original value of a outside that block too because a was declared with the `var` keyword.

#### Redeclaring a variable with `let` in a different scope or block treats that variable as a different variable. And the value of a variable outside does not change. like-

```javascript
let a = 5;
console.log(a); // 5
{
    let a = 1;
    console.log(a); // 1
}
console.log(a); // 5
```

#### The variables declared with `var` are hoisted to the top of the scope of the program. For example,

```javascript
console.log(a);    // undefined (not an error)
var a = 10;
```

#### The keyword `let` does not allow hoisting. For example,

```javascript
console.log(a);    // Uncaught ReferenceError: a is not defined
var a = 10;
```

I hope you all enjoyed this blog! Thank You