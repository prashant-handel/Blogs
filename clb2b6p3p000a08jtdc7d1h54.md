---
title: "Map, filter and reduce in JavaScript"
datePublished: Tue Nov 29 2022 14:22:52 GMT+0000 (Coordinated Universal Time)
cuid: clb2b6p3p000a08jtdc7d1h54
slug: map-filter-and-reduce-in-javascript
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1669735949084/c_wN8ZnGH.jpg
tags: javascript, html, html5, map, reduce

---

# Introduction

map, filter and reduce all these methods are only applicable upon an array. These methods are used for looping on the array one after the other. Each of these method returns a new array based on the result of the function.

# map()

The `map()` method is used for creating a new array from an existing one and apply a function to each one of the elements of the array. This does not change the original array elements.

## Syntax-

```javascript
let numbers = [1, 2, 3, 4, 5];
function double(x) {
return x * x;
}
const squareNumbers = numbers.map(double);
console.log(squareNumbers);
```

## Output-

![Screenshot 2022-11-29 184803.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1669728737592/H3IHYyppa.jpg align="left")

# filter()

The `filter()` method takes each element in an array and it applies a conditional statement against it. If this conditional returns true, the element gets pushed to the new array. If the condition returns false, the element does not get pushed into the new array.

The `filter()` method is used on an array of objects having name of students and their corresponding marks. We can easily make a new array of students having marks more than 90 applying `filter()` method on the array.

## Syntax-

```javascript
let students = [
    { name: 'Rohit', marks: 86 },
    { name: 'Jason', marks: 54 },
    { name: 'Rahul', marks: 96 },
    { name: 'Vinod', marks: 70 },
    { name: 'Aditya', marks: 90 }
  ];  
  let studentMarks = students.filter(student => student. marks >= 90);
  console.log(studentMarks);
```

## Output-

![Screenshot 2022-11-29 192422.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1669730295688/31iH7SiA4.jpg align="left")

# reduce()

The `reduce()` method is also applicable on the array. The `reduce()` method returns a single value after executing the function for each element of the array. The `reduce()` method for adding array elements and reducing that in a single number. We can define any initial value after the completion of the function separated by a `,` symbol.

```javascript
let numbers = [1,2,3,4,5];
let sum = numbers.reduce((a,b) => {return a + b}, 0);
console.log(sum);    // 15
```