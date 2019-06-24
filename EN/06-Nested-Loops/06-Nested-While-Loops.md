[slide]
# Nested While Loops
```js
// Outer Loop
while (condition) {      
   // Inner Loop 
   while (condition) {   
       // Statements
   }
}
```
[/slide]

[slide]
# Example: Nested While Loops
```js
let row = 1;
while (row <= 2) {
  console.log(`Row: ${row}`);
  let col = 1;
  while (col <= 3) {
    console.log(`  Column: ${col}`);
    col++;
  }
  row++;
}
```
```
// Output
Row: 1
  Column: 1
  Column: 2
  Column: 3
Row: 2
  Column: 1
  Column: 2
  Column: 3
```
[/slide]

[slide]
# Problem: Triangle of Stars with While
[code-task title="Triangle of Stars with While" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function triangleOfStars(height) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a function to print a **triangle of stars** as shown below. It: 
* Receives the **height** of a triangle from the console
* Prints a **triangle of stars** using **while** loops
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
# Solution: Triangle of Stars with While
[code-task title="Triangle of Stars with While" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function triangleOfStars(height) {
  let row = 1;
  while (row < height) {
    let col = 0;
    while (col++ < row) {
      // TODO: Print a row of asteriks("*")
      row++;
    }
  }
}
```
[/code-editor]
[task-description]
Write a function to print a **triangle of stars** as shown below. It: 
* Receives the **height** of a triangle from the console
* Prints a **triangle of stars** using **while** loops
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