[slide]
# Homework
Now, it's your turn to practice what you have learned in the training session.

We have prepared some simple problems for you to solve. If you struggle you can see the solution after each problem. 
[/slide]

[slide]
# Problem: Fruit or Vegetable
[code-task title="Fruit or Vegetable" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function fruitOrVegetable(input) {
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
function fruitOrVegetable(input) {
    let product = input.shift();
    switch (product) {
      case "cucumber":
      case "pepper":
      case "carrot":
        console.log("vegetable");
        break;
      case "banana":
      case "apple":
      case "kiwi":
      case "cherry":
      case "lemon":
      case "grapes":
        console.log("fruit");
        break;
      default:
        console.log("unknown");
        break;
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
function dayOfWeek(input) {
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
function dayOfWeek(input) {
  let day = Number(input.shift());
  switch (day) {
    case 1:
      console.log("Monday");
      break;
    case 2:
      console.log("Tuesday");
      break;
    case 3:
      console.log("Wednesday");
      break;
    case 4:
      console.log("Thursday");
      break;
    case 5:
      console.log("Friday");
      break;
    case 6:
      console.log("Saturday");
      break;
    case 7:
      console.log("Sunday");
      break;
    default:
      console.log("Error");
      break;
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
# Problem: Vowel or Consonant
[code-task title="Vowel or Consonant" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function vowelOrConsonant(input) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a program to check a letter for vowel or consonant:

* Read a letter from the English alphabet
* Print either "Vowel" or "Consonant"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|a|Vowel|
|E|Vowel|
|b|Consonant|
[/slide]

[slide]
# Solution: Vowel or Consonant
[code-task title="Vowel or Consonant" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function vowelOrConsonant(input) {
  let letter = input.shift();

  if (letter === 'A' || letter === 'a' ||
    letter === 'E' || letter === 'e' ||
    letter === 'I' || letter === 'i' ||
    letter === 'O' || letter === 'o' ||
    letter === 'U' || letter === 'u') {
    console.log("Vowel");
  } else {
    console.log("Consonant");
  }
}
```
[/code-editor]
[task-description]
Write a program to check a letter for vowel or consonant:

* Read a letter from the English alphabet
* Print either "Vowel" or "Consonant"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|a|Vowel|
|E|Vowel|
|b|Consonant|
[/slide]

[slide]
# Problem: Product of 3 Numbers
[code-task title="Product of 3 Numbers" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function productOfThreeNumbers(input) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Calculate the sign of the product of 3 numbers:

* Read 3 floating-point numbers
* Print the sign of the product of the entered 3 numbers: positive, negative or zero

Try to do this without multiplying the 3 numbers

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|negative|
|3||
|-1||
|-3|positive|
|-4||
|5||
[/slide]

[slide]
# Solution: Product of 3 Numbers
[code-task title="Product of 3 Numbers" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function productOfThreeNumbers(input) {
  let n1 = Number(input.shift());
  let n2 = Number(input.shift());
  let n3 = Number(input.shift());

  if (n1 === 0 || n2 === 0 || n3 === 0) {
    console.log("zero");
  } else {
    let negativeNumbersCount = 0;
    
    if (n1 < 0) {
      negativeNumbersCount++;
    }

    if (n2 < 0) {
      negativeNumbersCount++;
    }

    if (n3 < 0) {
      negativeNumbersCount++;
    }

    if (negativeNumbersCount % 2 === 0) {
      console.log("positive");
    } else {
      console.log("negative");
    }
  }
}
```
[/code-editor]
[task-description]
Calculate the sign of the product of 3 numbers:

* Read 3 floating-point numbers
* Print the sign of the product of the entered 3 numbers: positive, negative or zero

Try to do this without multiplying the 3 numbers

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|negative|
|3||
|-1||
|-3|positive|
|-4||
|5||
[/slide]

[slide]
# Problem: Sorted Numbers
[code-task title="Sorted Numbers" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function sortedNumbers(input) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a program, which checks for sorted 3 numbers:

* Read 3 real numbers
* Print "Ascending" if the numbers are in ascending order
* Print "Descending" if the numbers are in descending order
* Print "Not sorted" in any other case

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|Ascending|
|2||
|3||
|3|Not sorted|
|1||
|2||
[/slide]

[slide]
# Solution: Sorted Numbers
[code-task title="Sorted Numbers" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function sortedNumbers(input) {
    let n1 = Number(input.shift());
    let n2 = Number(input.shift());
    let n3 = Number(input.shift());

    if (n1 < n2 && n2 < n3) {
      console.log("Ascending");
    } else if (n1 > n2 && n2 > n3) {
      console.log("Descending");
    } else {
      console.log("Not sorted");
    }
}
```
[/code-editor]
[task-description]
Write a program, which checks for sorted 3 numbers:

* Read 3 real numbers
* Print "Ascending" if the numbers are in ascending order
* Print "Descending" if the numbers are in descending order
* Print "Not sorted" in any other case

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|Ascending|
|2||
|3||
|3|Not sorted|
|1||
|2||
[/slide]

[slide]
# Problem: Vacation Expenses
[code-task title="Vacation Expenses" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function vacationExpenses(input) {
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
# Sample Input and Output
|Input|Output|
|-----|------|
|Winter|180.00|
|Hotel||
|5||
[/slide]

[slide]
# Solution: Vacation Expenses
[code-task title="Vacation Expenses" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function vacationExpenses(input) {
    let season = input.shift();
    let accommodation = input.shift();
    let days = Number(input.shift());
    let totalPrice = 0;

    if (season === "Spring") {
      if (accommodation === "Hotel") {
        totalPrice = days * 30 * 0.80;
      } else if (accommodation === "Camping") {
        totalPrice = days * 10 * 0.80;
      }
    } else if (season === "Summer") {
      if (accommodation === "Hotel") {
        totalPrice = days * 50;
      } else if (accommodation === "Camping") {
        totalPrice = days * 30;
      }
    } else if (season === "Autumn") {
      if (accommodation === "Hotel") {
        totalPrice = days * 20 * 0.7;
      } else if (accommodation === "Camping") {
        totalPrice = days * 15 * 0.7;
      }
    } else if (season === "Winter") {
      if (accommodation === "Hotel") {
        totalPrice = days * 40 * 0.9;
      } else if (accommodation === "Camping") {
        totalPrice = days * 10 * 0.9;
      }
    }

    console.log(totalPrice.toFixed(2));
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
# Sample Input and Output
|Input|Output|
|-----|------|
|Winter|180.00|
|Hotel||
|5||
[/slide]

[slide]
# Problem: Cinema
[code-task title="Cinema" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function cinema(input) {
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
function cienema(input) {
    let type = input.shift();
    let rows = Number(input.shift());
    let cols = Number(input.shift());
    let seats = rows * cols;

    switch (type) {
      case "Premiere":
        console.log((seats * 12.0).toFixed(2));
        break;
      case "Normal":
        console.log((seats * 7.50).toFixed(2));
        break;
      case "Discount":
        console.log((seats * 5.00).toFixed(2));
        break;
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
function numberOperations(input) {
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
function numberOperations(input) {
    let num1 = Number(input.shift());
    let num2 = Number(input.shift());
    let operation = input.shift()

    let result = 0;
    if (operation === "+") {
      result = num1 + num2;
    } else if (operation === "-") {
      result = num1 - num2;
    } else if (operation === "*") {
      result = num1 * num2;
    } else if (operation === "/") {
      result = num1 / num2;
    } else if (operation === "%") {
      result = num1 % num2;
    }

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
function ATM(input) {
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
function ATM(input) {
  let balance = Number(input.shift());
  let withdraw = Number(input.shift());
  let limit = Number(input.shift());

  if (balance >= withdraw && withdraw <= limit) {
    Console.WriteLine("The withdraw was successful.");
  } else if (withdraw > limit) {
    Console.WriteLine("The daily limit was exceeded.");
  } else if (withdraw > balance) {
    Console.WriteLine("Insufficient availability.");
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

[slide]
# Problem: Biggest of Five Numbers
[code-task title="Biggest of Five Numbers" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function biggestOfFiveNumbers(input) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a program to find the biggest among 5 numbers
* Read 5 integers
* Print the biggest number
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|5|
|2||
|3||
|4||
|5||
|-1|-1|
|-2||
|-3||
|-4||
|-5||
[/slide]

[slide]
# Solution: Biggest of Five Numbers
[code-task title="Biggest of Five Numbers" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function biggestOfFiveNumbers(input) {
  let num1 = Number(input.shift());
  let num2 = Number(input.shift());
  let num3 = Number(input.shift());
  let num4 = Number(input.shift());
  let num5 = Number(input.shift());

  if (num1 >= num2 && num1 >= num3 && num1 >= num4 && num1 >= num5) {
    console.log(num1);
  } else if (num2 >= num1 && num2 >= num3 && num2 >= num4 && num2 >= num5) {
    console.log(num2);
  } else if (num3 >= num1 && num3 >= num2 && num3 >= num4 && num3 >= num5) {
    console.log(num3);
  } else if (num4 >= num1 && num4 >= num2 && num5 >= num3 && num4 >= num5) {
    console.log(num4);
  } else if (num5 >= num1 && num5 >= num2 && num5 >= num3 && num5 >= num4) {
    console.log(num5);
  }
}
```
[/code-editor]
[task-description]
Write a program to find the biggest among 5 numbers
* Read 5 integers
* Print the biggest number
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|5|
|2||
|3||
|4||
|5||
|-1|-1|
|-2||
|-3||
|-4||
|-5||
[/slide]