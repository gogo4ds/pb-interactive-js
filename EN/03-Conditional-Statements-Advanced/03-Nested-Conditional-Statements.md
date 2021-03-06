[slide]
# Nested Conditional Statements
An if...else statement can exist within another ***if...else*** statement

Generally used when we have to test one condition followed by another

It's not a good practice to exceed three **nested levels**

# Example
```js
if (raining) {
   if (haveUmbrella) {
      // take the umbrella
   }
} else {
   // don't take an umbrella
}
```
[/slide]

[slide]
# Problem: Marketplace
[code-task title="Marketplace" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function marketPlace(input) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Create a function, which:

* Receives a product and day
* Print the price, formatted to **2nd** digit, based on the price list:

|Product|Weekday|Weekend|
|-------|-------|-------|
|Banana|2.50|2.70|
|Apple|1.30|1.60|
|Kiwi|2.20|3.00|
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|Banana|2.50|
|Weekday||
[/slide]

[slide]
# Solution: Marketplace
[code-task title="Marketplace" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function marketPlace(input) {
  let product = input.shift();
  let dayOfWeek = input.shift();

  if (product == "Banana") {
    if (dayOfWeek == "Weekday") {
      console.log("2.50");
    } else
      console.log("2.70");
  } else if (product == "Apple") {
    if (dayOfWeek == "Weekday") {
      console.log("1.30");
    } else {
      console.log("1.60");
    }
  } else if (product == "Kiwi") {
    if (dayOfWeek == "Weekday") {
      console.log("2.20");
    } else {
      console.log("3.00");
    }
  }
}
```
[/code-editor]
[task-description]
Create a function, which:

* Receives a product and day
* Print the price, formatted to **2nd** digit, based on the price list:

|Product|Weekday|Weekend|
|-------|-------|-------|
|Banana|2.50|2.70|
|Apple|1.30|1.60|
|Kiwi|2.20|3.00|
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|Banana|2.50|
|Weekday||
[/slide]

[slide]
# Problem: Biggest Number of Three
[code-task title="Biggest Number of Three" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function biggestNumberOfThree(input) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives three numbers
* Prints the biggest one
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|3|
|2||
|3||
|-1|-1|
|-5||
|-9||
[/slide]

[slide]
# Solution: Biggest Number of Three
[code-task title="Biggest Number of Three" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function biggestNumberOfThree(input) {
  let first = Number(input.shift());
  let second = Number(input.shift());
  let third = Number(input.shift());

  if (first > second)
    if (first > third) {
      console.log(first);
    } else {
      console.log(third);
    } else
    if (second > third) {
      console.log(second);
    } else {
      console.log(third);
    }
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives three numbers
* Prints the biggest one
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|3|
|2||
|3||
|-1|-1|
|-5||
|-9||
[/slide]