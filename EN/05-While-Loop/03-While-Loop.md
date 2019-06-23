[slide]
# While Loop
The **`while`** statement executes a statement or a block of statements while a specified **`Boolean expression`** evaluates to **`true`**

The expression is evaluated before each execution of the loop

# Example: Print the numbers from 1 to 5
```js
let i = 1;
while (i <= 5) {
   console.log(i);
   i++;
}
```
[/slide]

[slide]
# Problem: Decreasing Numbers
[code-task title="Decreasing Numbers" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function decreasingNumbers (input) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a program, which:

* Receive a number
* Prints the numbers starting from the numbers to 1 (inclusive)
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|4|4|
||3|
||2|
||1|
|5|5|
||4|
||3|
||2|
||1|
[/slide]

[slide]
# Solution: Decreasing Numbers
[code-task title="Decreasing Numbers" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function decreasingNumbers (input) {
  let inputNumber = Number(input.shift());
  
  while (inputNumber >= 1) {
    console.log(inputNumber);
    number--;
  }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Receive a number
* Prints the numbers starting from the numbers to 1 (inclusive)
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|4|4|
||3|
||2|
||1|
|5|5|
||4|
||3|
||2|
||1|
[/slide]