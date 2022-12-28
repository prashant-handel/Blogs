# JavaScript Data Types

The Data type is an important concept in programming. We must be able to know about the data type of the variables for applying various operations on it. The computer is not able to solve problems without knowing the data type of the variables.

For example -

`let x = 56 * "Rohan";`

In the above problem, JavaScript will throw an error and it is not possible to solve that equation.

## JavaScript Strings

A string (or a text string) is a collection of characters which is used to create sentences or names or anything. We can perform various properties and methods on the string like length, indexOf(), substring etc. Strings are written with quotes. We can use single or double quotes.

#### Examples-

```javascript
let str1 = "Rohan";
let str2 = 'Rohan';
let str3 = "80";
let str4 = "Ravi is an intelligent boy."
```

# JavaScript Numbers

Numbers are the integral values in JavaScript. The numbers can be defined with or without decimal in JavaScript. The numbers with decimals are known as float values and without decimals are known as integers.

`let x1 = 97.00;     // Written with decimals`  
`let x2 = 97;        // Written without decimals`

Extra large or extra small numbers can be written with scientific (exponential) notation which are used in regular maths expressions-

`let y = 596e7;      // 5960000000`  
`let z = 596e-7;     // 0.0000596`

There are various operations that we can do on numbers. We can perform addition, division, subtraction, multiplication, greater than, less than and other various operations on the numbers in JavaScript.

# JavaScript Booleans

The Boolean values are of two types. It may be true or false. The Booleans are generally used in checking the conditions whether true or false.

```javascript
let x = 59;
let y = 59;
let z = 62;
(x == y)       // Returns true
(x == z)       // Returns false
```

# JavaScript Arrays

JavaScript arrays are written with square brackets. Array items are separated by commas. The index of array starts with 0, which means the first item is of index '0', second is of index '1 ', and so on.

`let squares = [1, 4, 9, 25, 36];`

There are various methods that we can apply on array. A few methods are length, substring, concat, push, shift, pop etc. We also have some iterating methods to iterate over each elements of an array one after the another and perform several task on them.

# JavaScript Objects

JavaScript objects are written with curly braces `{}`. Object properties are written as (key: value) pairs, separated by commas `,` .

`let student = {firstName: "Rohit", lastName: "Patel", age: 22, stream: "CS"};`

The object of student in the above example 4 key: value pairs: firstName, lastName, age, and stream.