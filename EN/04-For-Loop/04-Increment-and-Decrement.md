[slide]
# Increment / Decrement Operators
Increment (++) operator increases the value by 1

Decrement (--) operator decreases the value by 1

Can be used pre and post fix

* Prefix: ***++i***, ***--i***
* Postfix: ***i++***, ***i--***

Both operators can be used only with numeric variables

# Examples: 
Pre-decrement
```js
let a = 1; 
console.log(--a); // 0
console.log(a);   // 0
```
Post-decrement
```js
let a = 1; 
console.log(a--); // 1
console.log(a);   // 0
```
[/slide]

[slide]
# For Loop with Step
The step part in a for loop can either increase or decrease the value of a variable

```js
for (let i = 0; i < 10; i += 2) {
    console.log(i);
}
```
```js
for (let i = 10; i >= 0; i -= 2) {
  console.log(i);
}
```
[/slide]

[slide]
# Problem: Number Ending with 7
[code-task title="Number Ending with 7" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function numbersEndingWith7 (input) {
   // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a number n
* Prints all numbers from 7 to n, ending with 7
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|27|7|
||17|
||27|
|40|7|
||17|
||27|
||37|
[/slide]

[slide]
# Solution: Number Ending with 7
[code-task title="Number Ending with 7" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function numbersEndingWith7 (input) {
   let n = Number(input.shift());

   for (let i = 7; i <= n; i += 10) {
      console.log(i);
   }
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a number n
* Prints all numbers from 7 to n, ending with 7
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|27|7|
||17|
||27|
|40|7|
||17|
||27|
||37|
[/slide]

[slide]
# Problem: Exam Countdown
[code-task title="Exam Countdown" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function examCountdown (days) {
   // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a numbers - count of days before an exam
* For each day prints: "\{currentDay\} days before the exam"
* At the end prints: "The exam has come"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|3 days before the exam
||2 days before the exam|
||1 days before the exam|
||The exam has come|
[/slide]

[slide]
# Solution: Exam Countdown
[code-task title="Exam Countdown" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function examCountdown (input) {
   let days = Number(input.shift());

   for (let i = days; i >= 1; i -= 1) {
      console.log(`${i} days before the exam`);
   }
   
   console.log("The exam has come");
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a numbers - count of days before an exam
* For each day prints: "\{currentDay\} days before the exam"
* At the end prints: "The exam has come"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|3 days before the exam
||2 days before the exam|
||1 days before the exam|
||The exam has come|
[/slide]