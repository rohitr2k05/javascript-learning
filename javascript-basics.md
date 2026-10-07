JavaScript Basics

Start with this:

# JavaScript Learning

## 1. What is JavaScript?

JavaScript is a programming language used to make websites interactive and dynamic.

It is commonly used for:
- Web development
- Frontend development
- Backend development
- Web applications

Example:

```javascript
console.log("Hello World");

Output:
Hello World

2. How to Run JavaScript

JavaScript can be written inside an HTML file using the <script> tag.

Example:

<!DOCTYPE html>
<html>
<head>
    <title>JavaScript</title>
</head>
<body>

    <h1>Hello JavaScript</h1>

    <script>
        console.log("Hello World");
    </script>

</body>
</html>

JavaScript can also be written in a separate .js file.

Example:

<script src="script.js"></script>
3. Comments

Comments are used to explain code. They are not executed.

Single-line comment
// This is a comment
console.log("Hello");
Multi-line comment
/*
This is a
multi-line comment
*/
4. Variables

Variables are used to store data.

JavaScript has three ways to declare variables:

var
let
const
var
var name = "Rohit";
console.log(name);
let
let age = 21;
age = 22;

console.log(age);
const
const pi = 3.14;
console.log(pi);

let can be changed.

const cannot be reassigned.

Example:

let age = 21;
age = 22;

This is allowed.

const age = 21;
age = 22;

This gives an error.

Data Types

JavaScript has different types of data.

String

Used for text.

let name = "Rohit";
Number

Used for numbers.

let age = 21;
let price = 99.99;
Boolean

Stores true or false.

let isStudent = true;
let isLoggedIn = false;
Undefined

A variable that has been declared but has no value.

let x;

console.log(x);

Output:

undefined
Null

Represents an intentional empty value.

let value = null;
Object

Stores multiple values in key-value pairs.

let student = {
    name: "Rohit",
    age: 21
};
Array

Stores multiple values.

let fruits = ["Apple", "Mango", "Orange"];
7. typeof Operator

typeof is used to check the data type.

let name = "Rohit";
console.log(typeof name);

Output:

string

Example:

console.log(typeof 10);        // number
console.log(typeof "Hello");   // string
console.log(typeof true);      // boolean
8. Operators

Operators are used to perform operations on values.

Arithmetic Operators
Operator	Meaning
+	Addition
-	Subtraction
*	Multiplication
/	Division
%	Remainder
**	Power

Example:

let a = 10;
let b = 3;

console.log(a + b); // 13
console.log(a - b); // 7
console.log(a * b); // 30
console.log(a / b); // 3.333
console.log(a % b); // 1
console.log(a ** b); // 1000
9. Assignment Operators

Assignment operators are used to assign values.

let x = 10;

x += 5;  // x = x + 5
x -= 2;  // x = x - 2
x *= 2;  // x = x * 2
x /= 2;  // x = x / 2
10. Comparison Operators

Comparison operators compare two values.

let a = 10;
let b = 20;

console.log(a == b);   // false
console.log(a != b);   // true
console.log(a > b);    // false
console.log(a < b);    // true
console.log(a >= b);   // false
console.log(a <= b);   // true
== vs ===
==

Checks value after type conversion.

5 == "5"

Output:

true
===

Checks both value and data type.

5 === "5"

Output:

false
Recommended

Prefer:

===

over:

==

when writing modern JavaScript.

11. Logical Operators

Logical operators are used with multiple conditions.

AND &&

Both conditions must be true.

let age = 21;

console.log(age > 18 && age < 30);

Output:

true
OR ||

At least one condition must be true.

let age = 16;

console.log(age > 18 || age == 16);

Output:

true
NOT !

Reverses the result.

let isStudent = true;

console.log(!isStudent);

Output:

false
12. Increment and Decrement
Increment
let x = 5;

x++;
console.log(x);

Output:

6
Decrement
let x = 5;

x--;
console.log(x);

Output:

4
13. Taking Input

In a browser, prompt() can be used to take input.

let name = prompt("Enter your name");

console.log(name);

Example:

let age = prompt("Enter your age");

console.log(age);

Important:

prompt() normally returns the input as a string.

To convert it to a number:

let age = Number(prompt("Enter your age"));

console.log(age);
14. Type Conversion

Type conversion means converting one data type into another.

String to Number
let x = "10";

let number = Number(x);

console.log(number);
Number to String
let x = 10;

let text = String(x);

console.log(text);
To Boolean
let x = 1;

console.log(Boolean(x));
15. Strings

A string is a sequence of characters.

let name = "Rohit";

Strings can use:

"Hello"
'Hello'
`Hello`
String Concatenation

Joining strings together.

let firstName = "Rohit";
let lastName = "R";

let fullName = firstName + " " + lastName;

console.log(fullName);

Output:

Rohit R
16. Template Literals

Template literals use backticks.

let name = "Rohit";
let age = 21;

console.log(`My name is ${name} and I am ${age} years old.`);

Output:

My name is Rohit and I am 21 years old.

This is generally easier than using + for longer strings.

17. String Methods
length
let name = "Rohit";

console.log(name.length);
toUpperCase()
console.log(name.toUpperCase());
toLowerCase()
console.log(name.toLowerCase());
includes()
console.log(name.includes("oh"));
charAt()
console.log(name.charAt(0));
slice()
let text = "JavaScript";

console.log(text.slice(0, 4));

Output:

Java
18. Conditional Statements

Conditional statements are used to make decisions.

if
let age = 21;

if (age >= 18) {
    console.log("You are an adult");
}
if...else
let age = 16;

if (age >= 18) {
    console.log("Eligible");
} else {
    console.log("Not eligible");
}
if...else if...else
let marks = 75;

if (marks >= 90) {
    console.log("A+");
} else if (marks >= 75) {
    console.log("A");
} else if (marks >= 50) {
    console.log("B");
} else {
    console.log("Fail");
}
19. Ternary Operator

The ternary operator is a short way to write an if...else.

Syntax:

condition ? valueIfTrue : valueIfFalse;

Example:

let age = 20;

let result = age >= 18 ? "Adult" : "Minor";

console.log(result);
20. Switch Statement

switch is useful when checking one value against multiple cases.

let day = 2;

switch (day) {
    case 1:
        console.log("Monday");
        break;

    case 2:
        console.log("Tuesday");
        break;

    case 3:
        console.log("Wednesday");
        break;

    default:
        console.log("Invalid day");
}
21. Loops

Loops are used to repeat code.

JavaScript mainly has:

for loop
while loop
do...while loop
for Loop
for (let i = 1; i <= 5; i++) {
    console.log(i);
}

Output:

1
2
3
4
5
while Loop
let i = 1;

while (i <= 5) {
    console.log(i);
    i++;
}
do...while Loop

The code runs at least once.

let i = 1;

do {
    console.log(i);
    i++;
} while (i <= 5);
22. break

break stops a loop.

for (let i = 1; i <= 10; i++) {

    if (i == 5) {
        break;
    }

    console.log(i);
}

Output:

1
2
3
4
23. continue

continue skips the current iteration.

for (let i = 1; i <= 5; i++) {

    if (i == 3) {
        continue;
    }

    console.log(i);
}

Output:

1
2
4
5
24. Arrays

An array stores multiple values in a single variable.

let fruits = ["Apple", "Mango", "Orange"];

console.log(fruits);

Array indexes start from 0.

console.log(fruits[0]); // Apple
console.log(fruits[1]); // Mango
console.log(fruits[2]); // Orange
25. Array Methods
push()

Adds an element to the end.

let fruits = ["Apple", "Mango"];

fruits.push("Orange");

console.log(fruits);
pop()

Removes the last element.

fruits.pop();
unshift()

Adds an element to the beginning.

fruits.unshift("Banana");
shift()

Removes the first element.

fruits.shift();
length
console.log(fruits.length);
26. Looping Through an Array
let fruits = ["Apple", "Mango", "Orange"];

for (let i = 0; i < fruits.length; i++) {
    console.log(fruits[i]);
}
27. Functions

A function is a reusable block of code designed to perform a particular task.

Instead of writing the same code repeatedly, we can put it inside a function and call it whenever needed.

Function Declaration

Syntax:

function functionName() {
    // code
}

Example:

function greet() {
    console.log("Hello Rohit");
}

greet();

Output:

Hello Rohit
28. Function Parameters

Parameters allow us to pass information into a function.

function greet(name) {
    console.log(`Hello ${name}`);
}

greet("Rohit");
greet("John");

Output:

Hello Rohit
Hello John

Here:

name → parameter

"Rohit" → argument

29. Multiple Parameters

A function can have multiple parameters.

function add(a, b) {
    console.log(a + b);
}

add(10, 20);

Output:

30