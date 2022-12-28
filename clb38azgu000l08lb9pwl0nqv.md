# Difference Between "==" and "===" in JavaScript

# Introduction
This is a very confusing question among beginners 'What is the difference between "==" and "==="?'. Another question arises 'When to use "==" and when to use "===" operator?'. After reading this post you will be able to answer above questions easily. We will closely learn about the basic difference and need for both type of operators.

## Double Equals or Loose Equality (==)
The "==" is used when we have to check whether the values of both sides of the operator regardless of the type. Double equals "==" performs a type conversion if both sides are of different types, it will convert one side similar to the other one. Then, it will compare the values of both sides. If the values are similar then it will return true and if the values after conversion will not equal then it returns false.

## Triple Equals or Strict Equality (===)
The "===" is used when we have to check whether the values as well as type of both sides of values are same or not. Triple equals "===" does not perform any type conversion like the double equals operator. If the values are different then it will return false. And if type if different, then also it will return false. The triple equals "===" returns true only if both type and values of both sides are similar else it will return false.

## Examples-

```
console.log("Rohan" == "Rohan")    // true
console.log("Rohan" === "Rohan")    // true
console.log(78 == "78");    // true
console.log(78 === "78");    // false
console.log(0 == false)    // true
console.log(0 === false)    false
```

In the above examples, the first two conditions becomes true because the values and type of both sides of the operator are similar.

In the third condition, the 78 written without double quotes `"` is of type number. On the other side, the type of 78 within double quotes `"` is string. Thus in double equals comparison the string type is converted into the number type and then it will check whether both the values are same or not. Hence, in this case both the values are similar, it will return true.

In the forth condition, the type of both side values are not similar, therefore it will return false in the case of triple equals. 

The fifth condition is having number at one side and Boolean at the other side of the operator. In this case of double equals, the value of false will be converted into number i.e. 0 which then compares with the other side number which is also 0. Both the values are similar, thus it will return true.

The last condition is also having different type of values, therefore it will return false in the case of triple equals.