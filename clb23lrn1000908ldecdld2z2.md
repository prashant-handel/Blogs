---
title: "Console and some commonly used methods"
datePublished: Tue Nov 29 2022 10:50:38 GMT+0000 (Coordinated Universal Time)
cuid: clb23lrn1000908ldecdld2z2
slug: console-and-some-commonly-used-methods
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1669718977317/kqYmS8UL7.png
tags: javascript, console, html5, consolelog, window

---

# What is console?

A Web console is a tool which is mainly used to log information associated with a web page like: network requests, JavaScript, security errors, warnings, CSS etc. It enables us to interact with a web page by executing JavaScript expression in the contents of the page.

Various methods are used related to console, which are used for logging and various workings. The console is a global object that is accessible via the global scope of the browser window.

console.log() is one of the widely used method which is used with console in JavaScript. Many people don't know about other methods of console. I am going to share some most common methods of console.

## Commonly used methods?

### console.log()

The console.log() method is used to log output to the console of the browser. We can use any type of data within log() method, such as a string, array, integer, or object.

#### Syntax-

```javascript
console.log('I am coding legend')    // string
console.log([1,2,3,4]) //array
console.log({a:1, b:2}) //object 
console.log(5500)    // integer
console.log(true)    // boolean
console.log(null)
console.log(undefined)
```

#### Output-

![Screenshot 2022-11-29 160917.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1669718400936/QVqm73xoj.jpg align="left")

### console. clear()

The console.clear() method is used to clear the console. The console will the text ' Console was cleared' in the console after using this method.

#### Syntax-

```javascript
console.clear()
```

#### Output-

![Screenshot 2022-11-29 161128.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1669718498721/J6AzPeXZi.jpg align="left")

### console. warn()

This method is used to log warning messages in the console. This warning message will be highlighted with yellow color. e.g.-

#### Syntax

```javascript
console.warn('This is a warning')
```

#### Output-

![Screenshot 2022-11-29 161231.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1669718617278/LoTXIjogt.jpg align="left")

### console. error()

The console.error() method is used to log error message in the console. The error message will be highlighted in red color.

#### Syntax-

```javascript
console.error('This is an error')
```

#### Output-

![Screenshot 2022-11-29 161526.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1669718745805/9G-WOuhMI.jpg align="left")

### console. assert()

The console. assert() method is used whether we want to check a condition whether it is true or false. It gives an error message to the console if the assertion is false. If the assertion is true, nothing happens.

The syntax shows the working of the console.assert() which gives error while the number is not divisible by 3 and don't show error while it is divisible by 3method-

#### Syntax-

```javascript
const errorMsg = "The number is not divisible by 3.";
for (let number = 2; number <= 6; number++) {
  console.log(`The number is ${number}`);
  console.assert(number % 3 === 0, errorMsg);
}
```

#### Output-

![Screenshot 2022-11-29 160639.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1669718217187/W_buCVqSb.jpg align="left")

### console. dir()

The console.dir() method is used to display a list of the properties of the specified JavaScript object. This method recognizes the object as an object and prints its properties. This method displays the list of properties in the form of object representation or JSON representation from where we can check the element properties.

#### Syntax-

```javascript
let info = {
    "name": "Neeraj",
    "Social": "@neeraj02"
    }
    console.dir(info)
```

#### Output-

![Screenshot 2022-11-29 162433.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1669720356203/XmTrNc8Mo.jpg align="left")

### console. dirxml()

The console.dirxml() method is used to display a tree of the descendant elements of the specified XML/HTML element or object. This method displays the tree in the form of XML representation as a hierarchical form of expandable nodes that allow us to see the contents of child nodes.

#### Syntax-

```javascript
let info = {
    "name": "Neeraj",
    "Social": "@neeraj02"
    }
    console.dir(info)
```

#### Output-

![Screenshot 2022-11-29 165344.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1669721036669/tfQDcVGEk.jpg align="left")