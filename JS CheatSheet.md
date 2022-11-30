# Javascript Cheatsheet (Beginners)

## Comments

```javascript
// This is a one-line comment
/*
This is a multi-line comment
This line too
*/
```

## Variables

### Variable Creation

```javascript
let user = "John Doe";
let age = 42;
let isActive = true;
```

### Variable Datatypes

```javascript
let user = "John Doe"; // String
let age = 42; // Number
let isActive = true; // Boolean
```

### Variable Operations

```javascript
let x = 40;
let y = 10;
let sum = x + y;
let difference = x - y;
```

## Debugging

```javascript
let name = "John";
console.log(name);
console.log("Hello World");
```

## Conditional Statements

### if Statement

```javascript
if (country === "India") {
  console.log("Cool");
}
```

### if-else Statement

```javascript
let age = 18;
if (age >= 18) {
  console.log("You are eligible");
} else {
  console.log("You are not eligible");
}
```

### Nested if-else Statement

```javascript
let num = 50;
if (num > 50) {
  console.log("Number is greater than 50");
} else {
  if (num === 50) {
    console.log("Number is equal to 50");
  } else {
    console.log("Number is greater than 50");
  }
}
```

## Logical and Comparision Operators

### Logical OR (||)

```javascript
let age = 20;
if (age > 18 || age < 50) {
  console.log("You are selected");
}
```

### Logical AND (&&)

```javascript
let age = 10;
let gender = "male";
if (age > 18 && gender === "male") {
  console.log("You are eligible");
}
```

### Comparision Operators

```javascript
2 > 3; // false
2 < 3; // true
2 <= 2; // true
3 >= 2; // true
2 === 5; // false
2 !== 3; // true
1 + 2 === 4; // false
```

## Strings

### String Concatenation

```javascript
let firstName = "John";
let lastName = "Doe";
let fullName = firstName + " " + lastName; // John Doe
```

### String Transformation

#### Uppercase

```javascript
let name = "john doe";
name = name.toUpperCase(); // JOHN DOE
```

#### Lowercase

```javascript
let name = "JOHN DOE";
name = name.toLowerCase(); // "john doe"
```

## Arrays

### Array Declaration

```javascript
let myList = [];
let fruits = ["apples", "oranges", "bananas"];
```

### Access an Array

```javascript
fruits[0];
fruits[3];
```

### Update an Array Item

```javascript
fruits[1] = "Mango";
fruits[1] = 3;
```

## Loops

### While Loop

```javascript
let times = 0;
while (times < 10) {
  console.log(times);
  times = times + 1;
}
```

### forEach Loop

```javascript
let fruits = ["apples", "oranges", "bananas"];
fruits.forEach(function (fruit) {
  alert("I have " + fruit + " in my bag");
});
```

### do While Loop

```javascript
let times = 0;
do {
  console.log(times);
  times = times + 1;
} while (times < 10);
```

## Dates

### Get Current Date and Time

```javascript
let now = new Date();
```

### Get Data from Date

```javascript
let now = new Date();
now.getMinutes();
now.getHours();
now.getDate();
now.getDay();
now.getMonth();
now.getFullYear();
```

## Math Functions

### Round

```javascript
Math.round(4.7); // 5
```

### Floor

```javascript
Math.floor(4.7); // 4
```

### Ceil

```javascript
Math.ceil(4.7); // 5
```

### Min

```javascript
Math.min(2, 5, 1); // 1
```

### Max

```javascript
Math.max(2, 5, 1); // 5
```

### Random

```javascript
Math.random(); // 0.9182460305807105
```

## Alerts & Prompts

### Alert

```javascript
alert("Hi");
let name = "John";
alert(name);
```

### Prompt

```javascript
let firstName = prompt("What is your first name");
let lastName = prompt("What is your last name");
let fullName = firstName + " " + lastName;
alert(fullName);
```

## Functions

### Basic Function

```javascript
function sayName() {
  let name = prompt("What's your name?");
  alert(name);
}

sayName();
```

### Function with Parameters

```javascript
function fullName(firstName, lastName) {
  alert(firstName + " " + lastName);
}

let firstName = prompt("What's your first name?");
let lastName = prompt("What's your last name?");
fullName(firstName, lastName);
fullName("Kate", "Robinson");
```

### Function with Return Value

```javascript
function add(x, y) {
  return x + y;
}

let result = add(3, 4);
let result2 = add(result, 0);
console.log(result2);
```

## Selectors

### Get Element By ID

```javascript
let li = document.getElementById("list-element");
```

### Query Selector

```javascript
let li = document.querySelector("li");
let paragraph = document.querySelector("p");
```

### Query Selector All

```javascript
let list = document.querySelectorAll("li");
```

## Events

### Creating an Event Listener

```javascript
function sayHi() {
  alert("hi");
}

let element = document.querySelector("#city");
element.addEventListener("click", sayHi);
```

### Set Timeout

```javascript
function sayHello() {
  alert("Hello");
}
setTimeout(sayHello, 3000);
```

### Set Interval

```javascript
function sayHello() {
  alert("Hello");
}
setInterval(sayHello, 3000);
```
