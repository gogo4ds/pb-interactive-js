[slide]
# Simple Conditions: if-else
If the condition is **false**, we may execute another code using the **еlse** block
```js
if (condition) {
   // Condition is true
} else {
   // Condition is false
}
```
[/slide]

[slide]
# Blocks of Code
The curly brackets \{\} introduce a **block** (a group of commands)

In case the **if** statement does **not** have curly brackets, only the code on the **next line** will be executed
```js
let color = "red";
if (color == "red") 
  console.log("tomato");
else
  console.log("banana");
console.log("lemon"); // Always executed
```
[/slide]

[slide]
# Blocks of Code
```js
let color = "red";
if (color === "red") {
   console.log("tomato");
   console.log("strawberry"); 
} else {
   console.log("banana");
   console.log("lemon");
   console.log("pear");
} 
```
[/slide]

[slide]
# Problem: Even or Odd
[code-task title="Even or Odd" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```js
function evenOrOdd([num]) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which: 
* Receives a single number
* If it's even, print "**even**"
* If it's odd, print "**odd**"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|4|even|
|7|odd|
[/slide]

[slide]
# Solution: Even or Odd
[code-task title="Even or Odd" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```js
function evenOrOdd([num]) {
   if (Number(num) % 2 === 0) {
      console.log("even");
   } else {
      console.log("odd");
   }
}
```
[/code-editor]
[task-description]
Write a function, which: 
* Receives a single number
* If it's even, print "**even**"
* If it's odd, print "**odd**"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|4|even|
|7|odd|
[/slide]

[slide]
# Problem: Greater Number
[code-task title="Greater Number" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```js
function greaterNumber([num1, num2]) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which: 
* Receives **two numbers**
* Finds the greater number
* Prints "Greater number:\{\} " + the **greater** number
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|Greater number: 8|
|8||
[/slide]

[slide]
# Solution: Greater Number
[code-task title="Greater Number" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```js
function greaterNumber([num1, num2]) {
   if (Number(num1) > Number(num2)) {
      console.log("Greater number: " + num1);
   } else {
      console.log("Greater number: " + num2);
   }
}
```
[/code-editor]
[task-description]
Write a function, which: 
* Receives **two numbers**
* Finds the greater number
* Prints "Greater number:\{\} " + the **greater** number
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|Greater number: 8|
|8||
[/slide]
