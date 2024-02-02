# JavaScript Documentation **!!!UNDER CONSTRUCTION!!!**

## Table of Contents
- [Introduction](#introduction)
- [Variables](#variables)
- [Data Types](#data-types)
- [Operators](#operators)
- [Control Flow](#control-flow)
    - [If-Else](#if-else)
    - [else-if](#else-if)
    - [switch](#switch)
    - [while](#while)
    - [do-while](#dowhile)
    - [for](#for)
    - [for-of](#for-of)
    - [for-in](#for-in)
    - [break](#break)
    - [continue](#continue)
    - [labels](#labels)
- [Functions](#functions)
- [Arrays](#arrays)
- [Objects](#objects)
- [Classes](#classes)
- [Modules](#modules)
- [Promises](#promises)
- [Error Handling](#error-handling)
- [Regular Expressions](#regular-expressions)
- [DOM Manipulation](#dom-manipulation)
- [AJAX](#ajax)
- [JSON](#json)
- [Debugging](#debugging)
- [Best Practices](#best-practices)

## Introduction
JavaScript is a popular programming language used for both front-end and back-end web development. It is a versatile language that allows developers to create interactive and dynamic web pages. This documentation provides a comprehensive guide to JavaScript, covering topics such as variables, data types, operators, control flow, functions, arrays, objects, classes, modules, promises, error handling, regular expressions, DOM manipulation, AJAX, JSON, debugging, and best practices. Whether you are a beginner or an experienced developer, this documentation will help you enhance your JavaScript skills and build robust web applications.

---

## Variables

In JavaScript, variables are used to store and manipulate data. They are declared using the `var`, `let`, or `const` keyword, followed by the variable name.
The `var` keyword is used to declare a variable that can be reassigned later. The `let` keyword is used to declare a variable that can be reassigned later. The `const` keyword is used to declare a variable that cannot be reassigned later.

```javascript
var x = 1;
let y = 2;
const z = 3;
```

Variables can also be declared without assigning a value to them.

```javascript

var x;
let y;
const z;
```

`var` is the oldest way to declare variables in JavaScript.
Variables declared with var are function-scoped, meaning they are accessible within the function in which they are declared.
If a variable declared with var is defined outside of any function, it becomes a global variable and can be accessed from anywhere in the code.
var variables can be redeclared and reassigned within their scope.
Hoisting: Variables declared with var are hoisted to the top of their scope, which means they can be accessed before they are declared. However, their value will be undefined until they are assigned a value.


`let` was introduced in ES6 (ECMAScript 2015) as a replacement for var.
Variables declared with let are block-scoped, meaning they are only accessible within the block in which they are declared (a block is defined by curly braces {}).
let variables can be reassigned within their scope, but they cannot be redeclared in the same scope.
Hoisting: Like var, let variables are hoisted to the top of their scope, but unlike var, they are not initialized with a value. This means that if you try to access a let variable before it is declared, you will get a ReferenceError.
const:


`const` was also introduced in ES6.
Variables declared with const are block-scoped, just like let.
The value of a const variable cannot be reassigned once it is assigned. It is a constant.
const variables must be assigned a value when they are declared. If you try to declare a const variable without assigning a value, you will get a SyntaxError.
const variables cannot be redeclared or reassigned within their scope.
Hoisting: Like let, const variables are hoisted to the top of their scope, but they are not initialized with a value. Trying to access a const variable before it is declared will result in a ReferenceError.

---

## Data Types
Learn about the various data types in JavaScript.

---

## Operators
Discover the various operators used for arithmetic, comparison, logical operations, etc.

| Category | Operator | Description |
|----------|----------|-------------|
| Arithmetic | `+` | Addition |
| Arithmetic | `-` | Subtraction |
| Arithmetic | `*` | Multiplication |
| Arithmetic | `/` | Division |
| Arithmetic | `%` | Modulus (Remainder) |
| Arithmetic | `++` | Increment |
| Arithmetic | `--` | Decrement |
| Assignment | `=` | Simple assignment |
| Assignment | `+=` | Addition assignment |
| Assignment | `-=` | Subtraction assignment |
| Assignment | `*=` | Multiplication assignment |
| Assignment | `**=` | Exponentiation assignment |
| Assignment | `/=` | Division assignment |
| Assignment | `%=` | Modulus assignment |
| Assignment | `<<=` | Left shift assignment |
| Assignment | `>>=` | Right shift assignment |
| Assignment | `>>>=` | Unsigned right shift assignment |
| Assignment | `&=` | Bitwise AND assignment |
| Assignment | `^=` | Bitwise XOR assignment |
| Assignment | `|=` | Bitwise OR assignment |
| Comparison | `==` | Equal to |
| Comparison | `===` | Strict equality (equal value and equal type) |
| Comparison | `!=` | Not equal to |
| Comparison | `!==` | Strict inequality (not equal value or not equal type) |
| Comparison | `>` | Greater than |
| Comparison | `<` | Less than |
| Comparison | `>=` | Greater than or equal to |
| Comparison | `<=` | Less than or equal to |
| Logical | `??` | Nullish coalescing operator |
| Logical | `&&=` | Logical AND assignment |
| Logical | `||=` | Logical OR assignment |
| Logical | `??=` | Nullish coalescing assignment |
| Logical | `&&` | Logical AND |
| Logical | `||` | Logical OR |
| Logical | `!` | Logical NOT |
| Conditional | `? :` | Ternary Operator |
| Bitwise | `&` | Bitwise AND |
| Bitwise | `|` | Bitwise OR |
| Bitwise | `^` | Bitwise XOR |
| Bitwise | `~` | Bitwise NOT |
| Bitwise | `<<` | Left shift |
| Bitwise | `>>` | Right shift |
| Bitwise | `>>>` | Unsigned right shift |
| Bitwise | `**` | Exponentiation |
| Type | `typeof` | Check the type of a value |
| Instance | `instanceof` | Check if an object is an instance of a specific class |
| Property | `in` | Check if a property exists in an object |
| Property | `delete` | Delete a property from an object |

---

## Control Flow
Control flow is the order in which the computer executes statements in a script. Code is run in order from the first line in the file to the last line, unless the computer runs across structures that change the control flow, such as conditionals and loops.

## Conditional Statements




<details>
<summary id='if-else' >If-Else</summary>

The `if` statement executes a statement if a specified condition is truthy. If the condition is falsy, another statement can be executed.

```javascript
let x = 10;
if (x > 5) {
  console.log('x is greater than 5');
} else {
  console.log('x is not greater than 5');
}
// Output: x is greater than 5
```
</details>




<details>
<summary id='if-else' >Else-If</summary>

The `if-else if-else` statement executes a statement if a specified condition is truthy. If the condition is falsy, another statement can be executed. If none of the conditions are truthy, a default statement can be executed.

```javascript
let x = 10;
if (x > 5) {
  console.log('x is greater than 5');
} else if (x < 5) {
  console.log('x is less than 5');
} else {
  console.log('x is equal to 5');
}
// Output: x is greater than 5
```
</details>




<details>
<summary id='switch' >Switch</summary>

The `switch` statement evaluates an expression and executes a statement based on the value of the expression.

```javascript
let x = 10;
switch (x) {
  case 5:
    console.log('x is equal to 5');
    break;
  case 10:
    console.log('x is equal to 10');
    break;
  default:
    console.log('x is not equal to 5 or 10');
}
// Output: x is equal to 10

or

let fruit = 'Banana';
switch (fruit) {
    case 'Apple':
        console.log('Apple is $0.32');
        break;
    case 'Banana':
        console.log('Banana is $0.48');
        break;
    case 'Cherry':
        console.log('Cherry is $0.15');
        break;
    default:
        console.log('Sorry, we are out of ' + fruit + '.');
}
// Output: Banana is $0.48
```

explaination:
In the switch statement, if the variable fruit is equal to 'Apple', the code block under 'Apple' will run, and so on. The default keyword specifies the code to run if there is no case match.

</details>

## Loops

<details>
<summary id='for-loop'>For Loop</summary>

The `for` loop runs a block of code a specific number of times.

```javascript
for (let i = 0; i < 5; i++) {
    console.log(i);
}

// Output: 0 1 2 3 4
```
</details>

<details>
<summary id='while-loop'>While Loop</summary>

The `while` loop runs a block of code while a specified condition is true.

```javascript
let i = 0;
while (i < 5) {
    console.log(i);
    i++;
}

// Output: 0 1 2 3 4
```
</details>

<details>
<summary id='do-while-loop'>Do-While Loop</summary>

The `do-while` loop runs a block of code while a specified condition is true. It will always execute the code block at least once.

```javascript
let i = 0;
do {
    console.log(i);
    i++;
} while (i < 5);

// Output: 0 1 2 3 4
```
</details>

<details>
<summary id='for-of-loop'>For-Of Loop</summary>

The `for-of` loop iterates over iterable objects such as arrays, strings, etc.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];

for (let fruit of fruits) {
    console.log(fruit);
}

// Output: Apple Banana Cherry
```
</details>

<details>
<summary id='for-in'>For-In Loop</summary>

The `for-in` loop iterates over the properties of an object.

```javascript
let person = {
    name: 'John',
    age: 30,
    city: 'New York'
};

for (let key in person) {
    console.log(key + ': ' + person[key]);
}

// Output: name: John age: 30 city: New York
```
</details>

<details>
<summary id='break'>Break</summary>

The `break` statement terminates the current loop, switch, or label statement and transfers program control to the statement following the terminated statement.

```javascript
for (let i = 0; i < 5; i++) {
    if (i === 3) {
        break;
    }
    console.log(i);
}

// Output: 0 1 2
```
</details>

<details>
<summary id='continue'>Continue</summary>

The `continue` statement terminates execution of the statements in the current iteration of the current or labeled loop, and continues execution of the loop with the next iteration.

```javascript
for (let i = 0; i < 5; i++) {
    if (i === 3) {
        continue;
    }
    console.log(i);
}

// Output: 0 1 2 4
```
</details>

<details>
<summary id='labels'>Labels</summary>

Labels are used to identify loops and blocks of code. They can be used with break and continue statements to control the flow of the program.

```javascript
outerLoop: for (let i = 0; i < 5; i++) {
    innerLoop: for (let j = 0; j < 5; j++) {
        if (i === 3 && j === 3) {
            break outerLoop;
        }
        console.log(i, j);
    }
}

// Output: 0 0 0 1 0 2 0 3 1 0 1 1 1 2 1 3 2 0 2 1 2 2 2 3
```
</details>

---

## Functions
Understand how to define and use functions in JavaScript.

---

## Arrays
Learn about arrays and their manipulation in JavaScript.


### Array Creation Access and Update

create an array
```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
```

access an array item
```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits[1]);
// Output: Banana
```

update an array item
```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
fruits[1] = 'Blueberry';
console.log(fruits);
// Output: ['Apple', 'Blueberry', 'Cherry']
```

### Array Methods

<details>
<summary id='at'>at</summary>

The `at` method returns the array item at the specified index.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.at(0));
// Output: Apple
```
</details>

<details>
<summary id='concat'>concat</summary>

The `concat` method concatenates two arrays.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.concat(['Date', 'Elderberry']));
// Output: ['Apple', 'Banana', 'Cherry', 'Date', 'Elderberry']
```
</details>

<details>
<summary id='copyWithin'>copyWithin</summary>

The `copyWithin` method copies a sequence of array elements within the array.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.copyWithin(2, 0));
// Output: ['Apple', 'Banana', 'Apple']
```
</details>

<details>
<summary id='entries'>entries</summary>

The `entries` method returns a new Array Iterator object that contains the key/value pairs for each index in the array.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.entries());
// Output: Array Iterator {}
```
</details>

<details>
<summary id='every'>every</summary>

The `every` method tests whether all elements in the array pass the test implemented by the provided function. It returns a Boolean value.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.every(function(fruit) {
    return fruit === 'Apple';
}));
// Output: false
```
</details>

<details>
<summary id='fill'>fill</summary>

The `fill` method fills all the elements of the array with a static value.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.fill('Apple'));
// Output: ['Apple', 'Apple', 'Apple']
```
</details>

<details>
<summary id='filter'>filter</summary>

The `filter` method creates a new array with all elements that pass the test implemented by the provided function.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.filter(function(fruit) {
    return fruit === 'Apple';
}));
// Output: ['Apple']
```
</details>

<details>
<summary id='find'>find</summary>

The `find` method returns the value of the first element in the array that satisfies the provided testing function. Otherwise undefined is returned.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.find(function(fruit) {
    return fruit === 'Apple';
}));
// Output: Apple
```
</details>

<details>
<summary id='findIndex'>findIndex</summary>

The `findIndex` method returns the index of the first element in the array that satisfies the provided testing function. Otherwise -1 is returned.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.findIndex(function(fruit) {
    return fruit === 'Apple';
}));
// Output: 0
```
</details>

<details>
<summary id='flat'>flat</summary>

The `flat` method creates a new array with all sub-array elements concatenated into it recursively up to the specified depth.

```javascript
let fruits = ['Apple', ['Banana', 'Cherry']];
console.log(fruits.flat());
// Output: ['Apple', 'Banana', 'Cherry']
```
</details>

<details>
<summary id='flatMap'>flatMap</summary>

The `flatMap` method creates a new array with the results of calling a provided function on every element in the array, and then flattening the result by one level.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.flatMap(function(fruit) {
    return fruit + ' Pie';
}));
// Output: ['Apple Pie', 'Banana Pie', 'Cherry Pie']
```
</details>

<details>
<summary id='forEach'>forEach</summary>

The `forEach` method executes a provided function once for each array element.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
fruits.forEach(function(fruit) {
    console.log(fruit);
});
// Output: Apple Banana Cherry
```
</details>

<details>
<summary id='includes'>includes</summary>

The `includes` method determines whether an array includes a certain value among its entries, returning true or false as appropriate.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.includes('Apple'));
// Output: true
```
</details>

<details>
<summary id='indexOf'>indexOf</summary>

The `indexOf` method returns the first index at which a given element can be found in the array, or -1 if it is not present.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.indexOf('Apple'));
// Output: 0
```
</details>

<details>
<summary id='join'>join</summary>

The `join` method joins all elements of an array into a string.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.join(', '));
// Output: Apple, Banana, Cherry
```
</details>

<details>
<summary id='keys'>keys</summary>

The `keys` method returns a new Array Iterator object that contains the keys for each index in the array.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.keys());
// Output: Array Iterator {}
```
</details>

<details>
<summary id='lastIndexOf'>lastIndexOf</summary>

The `lastIndexOf` method returns the last index at which a given element can be found in the array, or -1 if it is not present.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry', 'Apple'];
console.log(fruits.lastIndexOf('Apple'));
// Output: 3
```
</details>

<details>
<summary id='map'>map</summary>

The `map` method creates a new array with the results of calling a provided function on every element in the array.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.map(function(fruit) {
    return fruit + ' Pie';
}));
// Output: ['Apple Pie', 'Banana Pie', 'Cherry Pie']
```
</details>

<details>
<summary id='pop'>pop</summary>

The `pop` method removes the last element from an array and returns that element.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.pop());
// Output: Cherry
```
</details>

<details>
<summary id='push'>push</summary>

The `push` method adds one or more elements to the end of an array and returns the new length of the array.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.push('Date'));
// Output: 4
```
</details>

<details>
<summary id='reduce'>reduce</summary>

The `reduce` method applies a function against an accumulator and each value of the array (from left-to-right) to reduce it to a single value.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.reduce(function(total, fruit) {
    return total + fruit;
}, 0));
// Output: AppleBananaCherry
```
</details>

<details>
<summary id='reduceRight'>reduceRight</summary>

The `reduceRight` method applies a function against an accumulator and each value of the array (from right-to-left) to reduce it to a single value.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.reduceRight(function(total, fruit) {
    return total + fruit;
}, 0));
// Output: CherryBananaApple
```
</details>

<details>
<summary id='reverse'>reverse</summary>

The `reverse` method reverses the order of the elements in an array.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.reverse());
// Output: ['Cherry', 'Banana', 'Apple']
```
</details>

<details>
<summary id='shift'>shift</summary>

The `shift` method removes the first element from an array and returns that element.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.shift());
// Output: Apple
```
</details>

<details>
<summary id='slice'>slice</summary>

The `slice` method returns a shallow copy of a portion of an array into a new array object.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.slice(1, 3));
// Output: ['Banana', 'Cherry']
```
</details>

<details>
<summary id='some'>some</summary>

The `some` method tests whether at least one element in the array passes the test implemented by the provided function. It returns a Boolean value.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.some(function(fruit) {
    return fruit === 'Apple';
}));
// Output: true
```
</details>

<details>
<summary id='sort'>sort</summary>

The `sort` method sorts the elements of an array in place and returns the array.

```javascript
let fruits = ['Cherry', 'Banana', 'Apple'];
console.log(fruits.sort());
// Output: ['Apple', 'Banana', 'Cherry']
```
</details>

<details>
<summary id='splice'>splice</summary>

The `splice` method changes the contents of an array by removing or replacing existing elements and/or adding new elements.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.splice(1, 0, 'Blueberry'));
// Output: []
```
</details>

<details>
<summary id='toLocaleString'>toLocaleString</summary>

The `toLocaleString` method returns a string representing the elements of the array.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.toLocaleString());
// Output: Apple,Banana,Cherry
```
</details>

<details>
<summary id='toString'>toString</summary>

The `toString` method returns a string representing the elements of the array.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.toString());
// Output: Apple,Banana,Cherry
```
</details>

<details>
<summary id='unshift'>unshift</summary>

The `unshift` method adds one or more elements to the beginning of an array and returns the new length of the array.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.unshift('Avocado'));
// Output: 4
```
</details>

<details>
<summary id='values'>values</summary>

The `values` method returns a new Array Iterator object that contains the values for each index in the array.

```javascript
let fruits = ['Apple', 'Banana', 'Cherry'];
console.log(fruits.values());
// Output: Array Iterator {}
```
</details>

---

## Objects
Explore objects and their properties in JavaScript.

## Classes
Learn about object-oriented programming in JavaScript using classes.

## Modules
Discover how to use modules to organize and reuse code in JavaScript.

## Promises
Learn about promises and asynchronous programming in JavaScript.

## Error Handling
JavaScript provides error handling capabilities with the try...catch statement.

<details>
<summary id='try-catch'>Try-Catch</summary>

The try block contains the code to be executed. If an error occurs while executing the code in the try block, the catch block is executed.

```javascript
try {
    console.log('Start of try runs');
    unicycle;
    console.log('End of try runs -- never reached');
} catch(err) {
    console.log('Error has occurred: ' + err);
} finally {
    console.log('This is always run');
}

// Output: Start of try runs Error has occurred: ReferenceError: unicycle is not defined This is always run
```
</details>

<details>
<summary id='finally'>Finally</summary>

The finally block contains code to be executed regardless of the try / catch result. It is always executed, even if an error occurs in the try block.

```javascript
try {
    console.log('Start of try runs');
    unicycle;
    console.log('End of try runs -- never reached');
} catch(err) {
    console.log('Error has occurred: ' + err);
} finally {
    console.log('This is always run');
}

// Output: Start of try runs Error has occurred: ReferenceError: unicycle is not defined This is always run
```
</details>

<details>
<summary id='throw'>Throw</summary>
The throw statement allows you to create a custom error. It can be used together with the try...catch statement to handle custom errors.

```javascript
try {
    let message = 'Start of try runs';
    console.log(message);
    throw new Error('Something went wrong');
    console.log('End of try runs -- never reached');
} catch(err) {
    console.log('Error has occurred: ' + err);
} finally {
    console.log('This is always run');
}

// Output: Start of try runs Error has occurred: Error: Something went wrong This is always run
```
</details>

<details>
<summary id='custom-errors'>Custom Errors</summary>
You can create custom errors by extending the Error class.

```javascript
class ValidationError extends Error {
    constructor(message) {
        super(message);
        this.name = 'ValidationError';
    }
}

let err = new ValidationError('Something went wrong');

console.log(err.message);

// Output: Something went wrong
```
</details>

---

## Regular Expressions
Explore regular expressions and their usage in JavaScript.

## DOM Manipulation
Learn how to manipulate the Document Object Model (DOM) using JavaScript.

## AJAX
Discover how to make asynchronous HTTP requests using JavaScript.

## JSON
Learn how to work with JSON data in JavaScript.

## Debugging
Explore different techniques and tools for debugging JavaScript code.

## Best Practices
Learn about best practices and coding conventions for writing clean and maintainable JavaScript code.
