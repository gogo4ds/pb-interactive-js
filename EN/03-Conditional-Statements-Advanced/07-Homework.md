[slide]
# Problem: Fruit or Vegetable
[code-task title="Fruit or Vegetable" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function fruitOrVegetable(food) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a single string: ***"fruit"*** or ***"vegetable"***
    * **Fruits**: banana, apple, kiwi, cherry, lemon, grapes
    * **Vegetables**: cucumber, pepper, carrot
* Prints: ***"vegetable"***, ***"fruit"*** or ***"unknown"***

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|lemon|fruit|
|carrot|vegetable|
[/slide]

[slide]
# Solution: Fruit or Vegetable
[code-task title="Fruit or Vegetable" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function fruitOrVegetable(product) {
  switch (product) {
    case "cucumber":
    case "pepper":
    case "carrot":
      console.log("vegetable");
      break;
    // TODO: Implement the other cases
  }
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a single string: ***"fruit"*** or ***"vegetable"***
    * **Fruits**: banana, apple, kiwi, cherry, lemon, grapes
    * **Vegetables**: cucumber, pepper, carrot
* Prints: ***"vegetable"***, ***"fruit"*** or ***"unknown"***

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|lemon|fruit|
|carrot|vegetable|
[/slide]

[slide]
# Problem: Day of Week
[code-task title="Day of Week" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function dayOfWeek(day) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a number the day of the week in range \[1..7\]
* Prints the name of the day
* Prints ***"Error"*** if the number is not in the given range print
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|Monday|
|9|Error|
[/slide]

[slide]
# Solution: Day of Week
[code-task title="Day of Week" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function dayOfWeek(day) {
    switch (day) {
    case 1: console.log("Monday"); break;
    case 2: console.log("Tuesday"); break;
    // TODO: Implement the other valid days
    default: console.log("Error"); break; 
   }
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a number the day of the week in range \[1..7\]
* Prints the name of the day
* Prints ***"Error"*** if the number is not in the given range print
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|Monday|
|9|Error|
[/slide]

[slide]
# Problem: Vacation Expenses
[code-task title="Vacation Expenses" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function vacationExpenses(season, accomodationType, days) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a **season, accommodation type** and **days**
* Prints the total expenses, formatted to the 2nd digit

|Season|Hotel|Camping|Discount|
|------|-----|-------|--------|
|Spring|30|10|20%|
|Summer|50|30|0%|
|Autumn|20|15|30%|
|Winter|40|10|10%|
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Solution: Vacation Expenses
[code-task title="Vacation Expenses" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function vacationExpenses(season, accomodationType, days) {
    let totalPrice = 0;
    if (season == "Spring") {
       if (accommodation == "Hotel") {
          totalPrice = days * 30 * 0.70;
       } else if (accommodation == "Camping") {
          totalPrice = days * 10 * 0.70;
       }
    }
    // TODO: Implement the other cases

}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a **season, accommodation type** and **days**
* Prints the total expenses, formatted to the 2nd digit

|Season|Hotel|Camping|Discount|
|------|-----|-------|--------|
|Spring|30|10|20%|
|Summer|50|30|0%|
|Autumn|20|15|30%|
|Winter|40|10|10%|
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Problem: Point in Rectangle
[code-task title="Point in Rectangle" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function pointInRectangle(x, y) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads the coordinates of a point - **x, y**
* Reads the coordinates of a rectangle - **x1, y1, x2, y2**
* If the point is inside prints ***"Inside"***
* If it isn't prints ***"Outside"***
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Solution: Point in Rectangle
[code-task title="Point in Rectangle" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function pointInRectangle(x, y) {
    if (x >= x1 && x <= x2 && y >= y1 && y <= y2) {
      console.log("Inside");
    }
    // TODO: outside condition
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads the coordinates of a point - **x, y**
* Reads the coordinates of a rectangle - **x1, y1, x2, y2**
* If the point is inside prints ***"Inside"***
* If it isn't prints ***"Outside"***
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Problem: Cinema
[code-task title="Cinema" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function cinema(type, rows, cols) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives the **type** of the movie, the **rows** and the **seats per row** in the cinema
* Prints the total income formatted to the 2nd digit after the decimal point
|Type|Price|
|----|-----|
|Premiere|12.00|
|Normal|7.50|
|Discount|5.00|
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Solution: Cinema
[code-task title="Cinema" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function cinema(type, rows, cols) {
    let totalSeats = rows * cols;
    switch (type) {
       case "Premiere":
          console.log("{0:f2}", totalSeats * 12.0);
          break;
       // TODO: Implement the other cases
    }

}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives the **type** of the movie, the **rows** and the **seats per row** in the cinema
* Prints the total income formatted to the 2nd digit after the decimal point
|Type|Price|
|----|-----|
|Premiere|12.00|
|Normal|7.50|
|Discount|5.00|
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Problem: Number Operations
[code-task title="Number Operations" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function numberOperations(num1, num2, operation) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives two real numbers and math operator
* The math operator could be: **"+", "-", "\/", "%" and "\*"**
* The output should be in the following format: "\{N1\} \{operator\} \{N2\} = \{result\}"

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10|10 + 12 = 22|
|20||
|+||
[/slide]

[slide]
# Solution: Number Operations
[code-task title="Number Operations" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function numberOperations(num1, num2, operation) {
    let result = 0;
    if (operation == "+") 
      result = num1 + num2; 
    // TODO: Implement the rest of operations
    console.log(`${num1} ${operation} ${num2} = ${result}`);

}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives two real numbers and math operator
* The math operator could be: **"+", "-", "\/", "%" and "\*"**
* The output should be in the following format: "\{N1\} \{operator\} \{N2\} = \{result\}"

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10|10 + 12 = 22|
|20||
|+||
[/slide]

[slide]
# Problem: ATM
[code-task title="ATM" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function ATM(accountAmount, withdrawAmount, dailyLimit) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives 3 **numbers**:
    * ***accountAmount***, ***withdrawAmount*** and ***dailyLimit***
* Checks if the account amount has the desired money and the daily limit is not exceeded
* Prints a different string depending on the result
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Problem: ATM
[code-task title="ATM" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function ATM(accountAmount, withdrawAmount, dailyLimit) {
    if (// Withdraw is possible) {
        console.log("The withdraw was successful.");
    } else if (// Daily limit exceeded) {
        console.log("The daily limit was exceeded.");
    } else if (// Not enough account balance) {
        console.log("Insufficient availability.");
    }
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives 3 **numbers**:
    * ***accountAmount***, ***withdrawAmount*** and ***dailyLimit***
* Checks if the account amount has the desired money and the daily limit is not exceeded
* Prints a different string depending on the result
[/task-description]
[code-io /]
[/code-task]
[/slide]