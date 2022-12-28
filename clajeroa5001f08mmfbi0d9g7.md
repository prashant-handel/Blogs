# Ternary Operator in JavaScript

The ternary operator is used when there are two possible outcomes of any condition i.e. true or false. We assign two codes to the operator, one for the condition if it is true and another for the condition if it is false. 

This operator contains a question mark `?` before that a condition is defined which we have to check. After the question mark there are two set of blocks which is separated by a colon `:`. The block of codes between the question mark and colon will be executed if the condition before the question mark becomes true. And the third block of code executes when the condition becomes false. 

The best use of ternary operator is used when we have to replace simple if/ else statement. for example-

```
// With if/else
const personName = person => {
  if (person) {
    return `Hello, ${person.name}! Have a Great Day`;
  } else {
    return "Welcome, Guest!";
  };
};

console.log(personName({ name: 'Rohan' }));     // Hello, ${person.name}! Have a Great Day
console.log(personName());                               // Welcome, Guest!


// With ternary operator
const personName = student => student ? `Hello, ${person.name}! Have a Great Day` : "Welcome, Guest!";

console.log(personName({ name: 'Rohan' })); // Hello, ${person.name}! Have a Great Day
console.log(personName()); // Welcome, Guest!
```

The ternary operator is also used as a chain of ternary operator. For example-

```
// With if/else if/else
const grade = mark => {
  if (mark > 100) {
    return;
  } else if (mark > 80) {
    return 'A';
  } else if (mark > 70) {
    return 'B';
  } else if (mark > 60) {
    return 'C';
  } else if (mark > 50) {
    return 'D';
  } else {
    return 'F';
  };
};

console.log(grade(100)); // A
console.log(grade(1000)); // undefined
console.log(grade(10)); // F

// With chained ternary operators
const grade = mark => mark > 100 ? undefined
                      : mark > 80 ? 'A'
                      : mark > 70 ? 'B'
                      : mark > 60 ? 'C'
                      : mark > 50 ? 'D'
                      : mark > 0 ? 'F'
                      : undefined;

console.log(grade(100)); // A
console.log(grade(1000)); // undefined
console.log(grade(10)); // F
console.log(grade(-6)); // undefined
```

The ternary operator makes the code more readable. It is also used to reduce the number of lines of the code.