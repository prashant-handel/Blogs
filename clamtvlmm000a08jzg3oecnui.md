# Type Conversion in JavaScript

We have various types of values in JavaScript i.e. ineger, float, string, array, boolean etc. We can convert any type of value in another type by using the methods shown below. Firstly we can write the name of the type (having first capital letter) of the value we want to get and then write the value within parenthesis after it. like


```
let Var = 34;
console.log(Var, typeof Var);    // 34 number

Var = String(34)
console.log(Var, typeof Var);    // 34 string
``` 

As similar to the above example we can also convert values to number. like

```
let Var = '34' ;
console.log(Var, typeof Var);    // 34 string

Var = Number(34) 
console.log(Var, typeof Var);    // 34 number
```

We can also convert boolean to integer or string, as shown

```
let Var = true ;
console.log(Var, typeof Var);    // true boolean

Var = Number(true) 
console.log(Var, typeof Var);    // 1 number

Var = Number(false)
console.log(Var, type of Var);    // 0 number

Var = String(true)
console.log(Var, type of Var);     // true string
```

In the above example  while converting the boolean to the number, it will convert true into number `1` and false into number `0`. And while converting the boolean into the string value it will give true and false as shown above.

For converting arrays into other types we have to do like this


```
let arr = [1,2,3,4,5];
console.log(arr, arr.length, type of arr);    // [1,2,3,4,5]    5    array

str = String(arr);
console.log(str, str.length, type of str);    // 1,2,3,4,5    9    string
``` 

In the above example of array to string type conversion, the array is having length of 5 items and when it is converted to the string type the length of the string becomes 9 because it also count the `,` of the string. While conversion the brackets got ignored.

We cannot convert any non number into a number because it will show an error the NaN which means Not a Number.

```
let string = '25';
console.log(string, type of string)    //    25  string

let num = Number(string);
console.log(num, type of num)    //    25  number

let string2 = '25de';
console.log(string2, type of string2)    //    25de  string

let num2 = Number(string2);      //
console.log(num2, type of num2)    //    NaN  number
```

## We also have another method for the type conversion of values.

```
let a = 25;
console.log(a, type of a);    // 25    number

console.log(a.toString());    // 25  It is of type string
```