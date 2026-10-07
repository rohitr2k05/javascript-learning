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