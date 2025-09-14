# JavaScript Complete Study Guide

This document is a comprehensive guide to **JavaScript (JS)**.  
It is designed as a one-stop reference for beginners and intermediate learners preparing for interviews or projects.


## Introduction
- JavaScript is a **high-level, interpreted, dynamically-typed** programming language.
- It is mainly used for **web development** (frontend & backend with Node.js).
- It adds **interactivity** to web pages.

---

## Basics

### What is JavaScript?
- Client-side scripting language (runs in browser).
- Also works on server (Node.js).

### Hello World
```html
<script>
  console.log("Hello World");
</script>
Variables
var a = 10;   // function-scoped (old, avoid using)
let b = 20;   // block-scoped
const c = 30; // block-scoped, cannot be reassigned
Data Types
Primitive: string, number, boolean, null, undefined, symbol, bigint
Non-primitive: object, array, function

------------------------------------------------------

Operators
Arithmetic: + - * / % **
Comparison: == != === !== < > <= >=
Logical: && || !
Assignment: = += -= *=
Ternary: condition ? value1 : value2
-----------------------------------------------------
Type Conversion
String(123);  // "123"
Number("456"); // 456
Boolean(0);   // false

------------------------------------------------------

Control Flow
Conditional Statements
if (x > 10) {
  console.log("Greater");
} else {
  console.log("Smaller");
}

---------------------------------------------------------------

Loops
for (let i=0; i<5; i++) { console.log(i); }
while (x < 5) { x++; }
do { x++; } while (x < 5);

Switch
switch(day) {
  case 1: console.log("Monday"); break;
  default: console.log("Invalid");
}

----------------------------------------------------------
Functions
Function Declaration
function greet(name) {
  return "Hello " + name;
}

Function Expression
const greet = function(name) { return "Hello " + name; };

Arrow Functions
const greet = (name) => `Hello ${name}`;

Default & Rest Parameters
function add(a=0, b=0) { return a+b; }
function sum(...nums) { return nums.reduce((a,b)=>a+b); }

Scope & Hoisting
Scope: where a variable is accessible.
Global, Function, Block
Hoisting: variable & function declarations are moved to top.

---------------------------------------------------------------
Objects & Arrays
Objects
const person = { name: "John", age: 25 };
console.log(person.name);

Arrays
const arr = [1,2,3];
Array Methods
push(), pop(), shift(), unshift()
map(), filter(), reduce()
forEach(), find(), includes()

Strings
let str = "Hello";
str.length;
str.toUpperCase();
str.includes("He");
str.slice(0,3);
str.replace("Hello","Hi");
ES6+ Features
let & const
Replaces var, block-scoped.
--------------------------------------------------------
Template Literals
let name = "John";
console.log(`Hello ${name}`);

Destructuring
const [a,b] = [1,2];
const {name, age} = {name:"John", age:25};

Spread & Rest
const arr = [1,2,3];
const copy = [...arr];
function sum(...nums) { }

Modules
// export.js
export const x = 10;

// import.js
import {x} from './export.js';

---------------------------------------------------
DOM Manipulation
Selecting Elements

document.getElementById("id");
document.querySelector(".class");
document.querySelectorAll("p");

Changing Content & Styles
element.textContent = "Hello";
element.style.color = "red";

Events
element.addEventListener("click", () => console.log("Clicked"));
Asynchronous JavaScript

Callbacks
function fetchData(cb) {
  setTimeout(() => cb("Data received"), 1000);
}

Promises
const promise = new Promise((resolve, reject) => {
  resolve("Success");
});
promise.then(res => console.log(res));

Async/Await
async function getData() {
  let res = await fetch("api/data");
  let data = await res.json();
  console.log(data);
}
---------------------------------------------------------------
Fetch API
fetch("https://jsonplaceholder.typicode.com/posts")
  .then(res => res.json())
  .then(data => console.log(data));

------------------------------------------------------
Error Handling
try {
  throw new Error("Something went wrong");
} catch (err) {
  console.log(err.message);
} finally {
  console.log("Always runs");
}

------------------------------------------------------------------------
Advanced Topics
Closures
A function that remembers its scope even after execution.

function outer() {
  let count = 0;
  return function inner() {
    count++;
    return count;
  }
}
const counter = outer();
console.log(counter()); // 1

--------------------------------------------------
this Keyword
Refers to the current execution context.

In browser: window
In object method: the object itself
--------------------------------------------------
Prototype & Inheritance
function Person(name) {
  this.name = name;
}
Person.prototype.sayHi = function() {
  console.log("Hi " + this.name);
};
Event Loop & Execution Context
JS is single-threaded.
Uses call stack + event loop + callback queue for async tasks.

-----------------------------------------------------
DSA with JavaScript

Array Problems
// Reverse an array
function reverseArray(arr) {
  return arr.reverse();
}

// Find max
function findMax(arr) {
  return Math.max(...arr);
}


String Problems
// Reverse string
function reverseString(str) {
  return str.split("").reverse().join("");
}

// Palindrome check
function isPalindrome(str) {
  return str === str.split("").reverse().join("");
}

Recursion
// Factorial
function factorial(n) {
  if (n===0) return 1;
  return n * factorial(n-1);
}

// Fibonacci
function fib(n) {
  if (n<=1) return n;
  return fib(n-1) + fib(n-2);
}

Searching & Sorting
// Binary Search
function binarySearch(arr, target) {
  let left=0, right=arr.length-1;
  while(left<=right) {
    let mid = Math.floor((left+right)/2);
    if(arr[mid]===target) return mid;
    else if(arr[mid]<target) left=mid+1;
    else right=mid-1;
  }
  return -1;
}

// Bubble Sort
function bubbleSort(arr) {
  for(let i=0;i<arr.length;i++) {
    for(let j=0;j<arr.length-i-1;j++) {
      if(arr[j]>arr[j+1]) {
        [arr[j],arr[j+1]]=[arr[j+1],arr[j]];
      }
    }
  }
  return arr;
}

---------------------------------------------------
Interview Questions
Difference between var, let, const.
What is hoisting?
Difference between == and ===.
Explain closures with an example.
Explain event loop.
Difference between synchronous & asynchronous JS.
Difference between function declaration & expression.
How does this work in JS?
Difference between map, forEach, and filter.
What is the difference between null and undefined?
-----------------------------------------------------
Resources
MDN JavaScript Docs
W3Schools JavaScript
JavaScript.info
Eloquent JavaScript (Book)
You Don’t Know JS (Book)

