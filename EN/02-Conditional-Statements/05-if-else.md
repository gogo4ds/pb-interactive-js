[slide]
# If...else Statement
In an if-else statement, **`if`** condition evaluates to **`true`**, the then-statement runs. If condition is false, the else-statement runs

Because condition can't be simultaneously true and false, the then-statement and the else-statement of an if-else statement can never both run

In an if statement that doesn't include an else statement, if condition is true, the then-statement runs. If condition is false, control is transferred to the next statement after the if statement

```js
if (condition) {
  // then-statement
  // Commands to be executed if the condition is true
} else {
  // else-statement
  // Commands to be executed if the condition is false
}
```
[/slide]

[slide]
# Blocks of Code
The curly brackets ***\{\}*** introduce a **block** (a group of commands)

In case the ***if*** statement does **not** have curly brackets, only the code on the **next line** will be executed

```js
let color = "red";
if (color == "red") 
  console.log("tomato");
else
  console.log("banana");
console.log("lemon"); // Always executed
```

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
function evenOrOdd(input) {
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
function evenOrOdd(input) {
  let num = Number(input.shift());
   if (num % 2 === 0) {
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
function greaterNumber(input) {
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
function greaterNumber(input) {
  let num1 = Number(input.shift());
  let num2 = Number(input.shift());
  if (num1 > num2) {
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
