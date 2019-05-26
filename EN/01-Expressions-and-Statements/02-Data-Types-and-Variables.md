[slide]
# Variables and Data Types
# Variables
Variables == named area of the computer memory
  * Stores value of a certain type 
  * Accessible in the program by name
  * Container for data
    * The data can be read and changed at any time
  
**Variables** provide means for:
  * **Storing** data
  * **Retrieving** stored data
  * **Modifying** stored data
  
Variables are characterized by:
  * name (identifier)
  * type (of the information preserved)
  * value (stored information)

# Assigning Values to Variables
You can assign value to a variable using "**=**":
```js
let firstNum = 10;
let secondNum = 5;
let sum = firstNum + secondNum;
```

# Data Types
Six data types that are primitives:
* Boolean - true or false
* Null
* Undefined    
* Number - 1, 2, 4.5, -2        
* String - "Hello, World!"
* Symbol (new in ECMAScript 6)

# Data Types are Dynamic
In JavaScript data types are dynamic

A single variable can be used to hold different data types:
```js
let x = 5;   // x is Number
x = "John";  // x is String
x = true;  // x is Boolean
```

[/slide]

[slide]
# Log Variables on the Console
The console is useful for testing purposes

The **`console.log()`** method writes a message to the console:
```js
let firstNum = 10;
let secondNum = 5;
console.log(firstNum + secondNum); // 15
```
[/slide]

[slide]
# Read User Input
Use functions:
```js
function printNum (number) {
   console.log(number);
}
```

Call the function by name
```js
printNum(5);  // 5
printNum(10); //10
```

# Passing Multiple Parameters to a Function
You can pass multiple parameters to a function:
```js
function printSum (firstNum, secondNum) {
   console.log(firstNum, secondNum);
}

printSum(5, 10);       // 15
console.log(firstNum); // undefined
```
[/slide]

[slide]
# String Interpolation
Еnclosed by the back-tick (**\` \`**) character instead of double or single quotes

May contain placeholders which are indicated by the dollar sign and curly braces (**`${expression}`**):
```js
let name = "John"; 
console.log(`Hi, ${name}`);
```
[/slide]

[slide]
# Problem: Greeting
[code-task title="Greeting" executionStrategy="javascript-code" requiresInput]
[code-editor language="javascript"]
```
function sayHello (input) {
   // Write your code here
}
```
[/code-editor]
[task-description]
Create a function that:

* Receives a name
* Prints "Hello, \{name\}" on the console
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Solution: Greeting
[code-task title="Greeting" executionStrategy="javascript-code" requiresInput]
[code-editor language="javascript"]
```
function sayHello (input) {
  let user = input.shift();
  console.log(`Hello, ${user}`);
}
```
[/code-editor]
[task-description]
Create a function that:

* Receives a name
* Prints "Hello, \{name\}" on the console
[/task-description]
[code-io /]
[/code-task]
[/slide]