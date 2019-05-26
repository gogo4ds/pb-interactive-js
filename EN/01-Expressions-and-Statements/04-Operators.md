[slide]
# Arithmetic Operators
There are several arithmetic operators:

* "+" - addition
```js
let a = 5;
let b = 7;
let sum = a + b;
console.log(sum); // 12 
```

* "-" - subtraction
```js
let a = 15;
let b = 7;
console.log(a - b); // 8
```

* "*" - multiplication
```js
let a = 5;
let b = 7;
console.log(a * b); // 35
```

* "/" - division
```js
let a = 25;
console.log(a / 4); // 6.25
```

* "%" - modulus
```js
console.log(3 % 2);   // 1
console.log(4 % 2);   // 0
console.log(3.5 % 1); // 0.5
```
[/slide]

[slide]
# Problem: Area of Triangle
[code-task title="Area of Triangle" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function printTriangleArea(input) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Create a function that receives two parameters:

* The side of a triangle - a
* The height for that side - ha
* Print the area formatted to the 2nd digit
* Hint: use the "toFixed" method for formatting
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|25.00|
|10||
[/slide]

[slide]
# Solution: Area of Triangle
[code-task title="Area of Triangle" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function printTriangleArea(input) {
  let a = Number(input.shift());
  let h = Number(input.shift());
  let area = a * h / 2;
  console.log(area.toFixed(2));
}
```
[/code-editor]
[task-description]
Create a function that receives two parameters:

* The side of a triangle - a
* The height for that side - ha
* Print the area formatted to the 2nd digit
* Hint: use the "toFixed" method for formatting
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|25.00|
|10||
[/slide]
