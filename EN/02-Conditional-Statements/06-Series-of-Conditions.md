[slide]
# Sequence of If-Else Conditions
Sometimes we need to do a sequence of conditions before we decide what actions our program will execute. In such cases, we can apply the construction if-else if ... -else in series. For this purpose, we use the following format:

```js
if (…) {
  // code
} else if (…) { 
  // code
} else if (…) { 
  // code
}
```
[/slide]

[slide]
# Sequence of If-Else Conditions – Example
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
function printNumberValue(input) {
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
function printNumberValue(input) {
  let num = Number(input.shift());
  if (num == 1) {
      console.log("one");
  } else if (num === 2) {
      console.log("two");
  } else if (num === 3) {
      console.log("three");
  } else if (num === 4) {
      console.log("four");
  } else if (num === 5) {
      console.log("five");
  } else if (num === 6) {
      console.log("six");
  } else if (num === 7) {
      console.log("seven");
  } else if (num === 8) {
      console.log("eight");
  } else if (num === 9) {
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
