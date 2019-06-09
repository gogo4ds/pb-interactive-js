[slide]
# Logical Operators
Logical Operators are used to perform the logical operation between two operands like **AND**, **OR** and **NOT** based on our requirements

The Logical Operators will **always work with Boolean expressions** (**true** or **false**) and return **Boolean values**

The logical operators are:
  * AND (**&&**) - **returns true if both operands are true**
  * OR (**\| \|**) - **returns true if any one operand is true**
  * Logical negation (**!**) - **returns the reverse of logical state**
    * Brackets **()** change the order

| Operand1 | Operand2 | And | Or |
|---|---|---|---|
| true | true | true | true |
| true | false | false | true |
| false | true | false | true |
| false | false | false | false |

If you observe above table, **if any one operand value become false, then the logical AND operator will return false**, same way **the logical OR operator will return true, if any one operand value become true**

| Operand | Not |
|---|---|
| true | false |
| false | true |

If you observe above table, **the NOT operator will always return the reverse value of operand** like **if operand value true, then the Logical NOT operator will return false and vice versa**
[/slide]

[slide]
# Problem: Bonus Points
[code-task title="Bonus Points" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
function bonusPoints(input) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a program that applies bonus to given points
  * If points are between 0 and 3, adds 5
  * If points are between 4 and 6, adds 15
  * If points are between 7 and 9, adds 20
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|4|19|
[/slide]

[slide]
# Solution: Bonus Points
[code-task title="Bonus Points" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function bonusPoints(input) {
    let points = Number(input.shift());

    if (points >= 0 && points <= 3) {
      points += 5;
    } else if (points >= 4 && points <= 6) {
      points += 15;
    } else if (points >= 7 && points <= 9) {
      points += 20;
    }

    console.log(points);
}
```
[/code-editor]
[task-description]
Write a program that applies bonus to given points
  * If points are between 0 and 3, adds 5
  * If points are between 4 and 6, adds 15
  * If points are between 7 and 9, adds 20
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|4|19|
[/slide]


[slide]
# Problem: Food or Drink
[code-task title="Food or Drink" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function foodOrAnimal(input) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a program, which:
  * Reads single line and print "***drink***", "***food***" or "***unknown***"
  * Foods: curry, noodles, sushi, spaghetti 
  * Drinks: tea, water, coffee
  * Everything else is unknown
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Solution: Food or Drink
[code-task title="Food or Drink" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function foodOrAnimal(input) {
    let s = input.shift();
    if (s == "curry" || s == "noodles" || s == "sushi" || s == "spaghetti") {
      console.log("food");
    } else if (s == "tea" || s == "water" || s == "coffee") {
      console.log("drink");
    } else {
      console.log("unknown");
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

  * Reads single line and print "***drink***", "***food***" or "***unknown***"
  * Foods: curry, noodles, sushi, spaghetti 
  * Drinks: tea, water, coffee
  * Everything else is unknown
[/task-description]
[code-io /]
[/code-task]
[/slide]