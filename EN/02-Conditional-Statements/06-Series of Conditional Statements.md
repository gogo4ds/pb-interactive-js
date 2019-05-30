[slide]
# Series of Conditions
The **if-else** statement can be in a series
```js
if (…) 
  // code
else if (…) 
  // code
else if (…) 
  // code
```
If one condition is true, the program will **NOT check** the rest of the conditions
[/slide]

[slide]
# Series of Conditions – Example
The program checks the first condition, finds that it is **true** and ends
```js
let a = 7;
if (a > 4) 
  console.log("Bigger than 4"); 
else if (a > 5)
  console.log("Bigger than 5"); 
else 
  console.log("Smaller or equal to 4"); 
// The output is only "Bigger than 4" 
```
[/slide]

[slide]
# Problem: Number 1...9
[code-task title="Number 1...9" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```js
function printNumberValue([num]) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which: 
* Receives a single parameter and checks its value [1, 9]
* Prints the value in the form of text
* If the number is **greater** than 9 prints "**Number too big**"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|7|seven|
|10|Number too big|
[/slide]

[slide]
# Problem: Number 1...9
[code-task title="Number 1...9" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```js
function printNumberValue([num]) {
    if (Number(num) == 1) {
       console.log("one");
    } else if (Number(num) === 2) {
       console.log("two");
    } else if (Number(num) === 3) {
       console.log("three");
    } else if (Number(num) === 4) {
       console.log("four");
    } else if (Number(num) === 5) {
       console.log("five");
    } else if (Number(num) === 6) {
       console.log("six");
    } else if (Number(num) === 7) {
       console.log("seven");
    } else if (Number(num) === 8) {
       console.log("eight");
    } else if (Number(num) === 9) {
       console.log("nine");
    } else {
       console.log("Number too big");
    }
}
```
[/code-editor]
[task-description]
Write a function, which: 
* Receives a single parameter and checks its value [1, 9]
* Prints the value in the form of text
* If the number is **greater** than 9 prints "**Number too big**"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|7|seven|
|10|Number too big|
[/slide]
