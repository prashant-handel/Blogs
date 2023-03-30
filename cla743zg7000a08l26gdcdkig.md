---
title: "Conditional Statements"
datePublished: Mon Nov 07 2022 18:23:56 GMT+0000 (Coordinated Universal Time)
cuid: cla743zg7000a08l26gdcdkig
slug: conditional-statements
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1680176196301/3416f6e1-8786-4405-8006-6c2d83b3ef73.jpeg
tags: javascript, html, html5, javascript-framework, conditional

---

There are various types of conditional statements in JavaScript, like-

1. If Statement
    
2. If-else Statement
    
3. If-elseif-else Statement
    

**If Statement**

The if statement is used when we have to check any condition if it is true or false. If the given condition satisfies then the code within the if statement block executes. And if the condition does'nt satisfies then the code within the block does'nt execute and the control ran out of the if block.

for example-

```javascript
let x = 5;
if(x<10){
console.log(`${x} is less than 10`);
}
```

The condition in the above case i.e. x&lt;10 satisfies so the code within the block executes and gives output in the console.

**If-else Statement**

The if else statement consists of 2 blocks (one block of if statement and other block of else statement). The if block consists of if statement with condition, if the condition satisfies the codes within the if block executes. And if the condition does'nt satisfies, then the code within the else block executes.

for example-

```javascript
let x = 5;
if(x<3){
console.log(`${x} is less than 3`);
}
else{
console.log(`${x} is not less than 3`);
}
```

The above condition in the if statement block i.e. x&lt;3 does'nt satisfies so the control goes into the else statement's block and the code within the block executes and gives output in the console.

**If-elseif-else Statement**

The if-elseif-else statement consists of 3 blocks (one block of if statement, other block(s) of elseif statement(s) and one block of else statement at the last). The if block consists of if statement with condition, if the condition satisfies then the codes within the if block executes. And if the condition does'nt satisfies, then it will check for the next elseif condition and so own. At last, we have to provide the else block of the code. If the condition of if block and all elseif blocks does'nt satisfies the code within the else block executes.

for example-

```javascript
let x = 5;
if(x==3){
console.log(`${x} is equal to 3`);
}

else if(x==4){
console.log(`${x} is equal to 4`);
}

else if(x==5){
console.log(`${x} is equal to 5`);
}

else if(x==6){
console.log(`${x} is equal 6`);
}

else{
console.log(`${x} is greater than 6`);
}
```

In the above statements, the checking of the conditions will be done in the sequential manner. First of all, the condition of if statement checked, if it satisfies then the code within the block executes and if the condition does'nt satisfied then it will check for another condition and so own... If all else if conditions are not satisfied then finally the else block code executes the control ran out of the statement.