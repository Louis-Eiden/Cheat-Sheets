# JavaScript Documentation


<details>
<summary>Introduction</summary>

JavaScript is a programming language that is used to create interactive effects within web browsers. It is a high-level, dynamic, weakly typed, prototype-based, multi-paradigm, and interpreted programming language. Alongside HTML and CSS, JavaScript is one of the three core technologies of the World Wide Web. JavaScript enables interactive web pages and is an essential part of web applications. The vast majority of websites use it for client-side page behavior, and all major web browsers have a dedicated JavaScript engine to execute it.

</details>

<details>
<summary>History</summary>

JavaScript was initially created to “make web pages alive”. The programs in this language are called scripts. They can be written right in a web page’s HTML and run automatically as the page loads.

</details>

<details>
<summary>ECMAScript</summary>

ECMAScript is a standard for a scripting language. It is a trademark scripting language specification standardized by Ecma International in ECMA-262 and ISO/IEC 16262. It was created to standardize JavaScript, so as to foster multiple independent implementations. JavaScript has remained the best-known implementation of ECMAScript since the standard was first published, with other well-known implementations including JScript and ActionScript. ECMAScript is commonly used for client-side scripting on the World Wide Web, and it is increasingly being used for writing server applications and services using Node.js.

</details>

<details>

<summary>Tools</summary>

</details>

<details>
<summary>Variables</summary>

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
</details>

<details>
<summary>Data Types</summary>

</details>

<details>
<summary>Operators</summary>

</details>

<details>
<summary>Control Flow</summary>
Control flow refers to the order in which statements are executed in a program. In JavaScript, control flow is determined by conditional statements and loops.
<details>
<summary>If-Else</summary>
</details>

<details>
<summary>Else-If</summary>

</details>


</details>