[slide]
# Nested For Loops
The syntax for **a nested for loop** in JS is as follows:
```js
// Outer Loop
for (init; condition; increment) {
  // Inner Loop
  for (init; condition; increment) { 
      // Commands
  }
}
```
[/slide]

[slide]
# Example: Nested For Loops
```js
let rows = 3;
let columns = 2;
for (let r = 1; r <= rows; r++) {
  console.log("row = " + r);
  for (let c = 1; c <= columns; c++) 
    console.log("  column = " + c);
}
```
```
row = 1
  column = 1
  column = 2
row = 2
  column = 1
  column = 2
row = 3
  column = 1
  column = 2
```
[/slide]

[slide]
# Problem: Triangle of Stars
[code-task title="Triangle of Stars" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function triangleOfStars(size) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a function to print a **triangle of stars** as shown below. It: 
* Receives the **size** of a triangle from the console
* Prints a **triangle of stars**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|\*|
||\*\*|
||\*\*\*|
||\*\*\*\*|
||\*\*\*\*\*|
|7|\*|
||\*\*|
||\*\*\*|
||\*\*\*\*|
||\*\*\*\*\*|
||\*\*\*\*\*\*|
||\*\*\*\*\*\*\*|
[/slide]

[slide]
# Solution: Triangle of Stars
[code-task title="Triangle of Stars" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function triangleOfStars(size) {
  let result = '';
  for (let row = 1; row <= size; row++) {
    for (let col = 1; col <= row; col++) {
      result += "*";
    }
    result += '\n';
  }
  console.log(result);
}
```
[/code-editor]
[task-description]
Write a function to print a **triangle of stars** as shown below. It: 
* Receives the **size** of a triangle from the console
* Prints a **triangle of stars**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|\*|
||\*\*|
||\*\*\*|
||\*\*\*\*|
||\*\*\*\*\*|
|7|\*|
||\*\*|
||\*\*\*|
||\*\*\*\*|
||\*\*\*\*\*|
||\*\*\*\*\*\*|
||\*\*\*\*\*\*\*|
[/slide]