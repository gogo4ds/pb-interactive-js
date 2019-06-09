[slide]
# Definition and Types
Very often when in your code, you want to perform different actions for different decisions

In JavaScript we have the following conditional statements:

* ***if*** - execute a block code, if a specified condition is true
* ***else*** - execute a block of code, if the same condition is false
[/slide]

[slide]
# The if Statement
Used to execute block of code if a given condition is met

```js
function greet (hour) {
  if (hour < 18) {
     console.log("Good day");
  }
}
greet(10);   // Good day
greet(19);   // No output
```
[/slide]

[slide]
# The else Statement
Used to execute block of code if a given condition is not met

```js
function greet (hour) {
  if (hour < 18) {
     console.log("Good day");
  } else {
     console.log("Good evening");
  }
}
greet(19); // Good evening
```
[/slide]

[slide]
# The else-if Statement
Used to chain multiple checks

```js
function greet (hour) {
  if (hour < 10) {
     console.log("Good morning");
  } else if (hour < 18) {
     console.log("Good day");
  } else {
     console.log("Good evening");
  }
}
```
[/slide]