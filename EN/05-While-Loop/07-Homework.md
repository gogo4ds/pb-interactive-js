[slide]
# Problem: Sum Digits
[code-task title="Sum Digits" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function sumDigits(input) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a function to sum the digits of given number

* Receives a number
* **Sum** its **digits** and print the sum
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5634|18|
|150|6|
|-532|10|
[/slide]

[slide]
# Solution: Sum Digits
[code-task title="Sum Digits" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function sumDigits(input) {
  let n = Number(input.shift());
  let sum = 0;

  while (n > 0) {
    sum += n % 10;
    n = Math.floor(n / 10);
  }

  console.log(sum);
}
```
[/code-editor]
[task-description]
Write a function to sum the digits of given number

* Receives a number
* **Sum** its **digits** and print the sum
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5634|18|
|150|6|
|-532|10|
[/slide]

[slide]
# Problem: Favorite Book
[code-task title="Favorite Book" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function favoriteBook(input) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which: 

* Receives a favorite book's name
* Receives books names until it gets the favorite book
* Prints:
    * "Book found!" and stops afterwards
    * "Invalid book: " + book for all invalid books
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|Alice in Wonderland|Book Found!|
|Winnie the Pooh||
|Alice in Wonderland||
[/slide]

[slide]
# Solution: Favorite Book
[code-task title="Favorite Book" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function favoriteBook(input) {
  let favoriteBook = books.shift();
  let book = input.shift();

  while (book !== favoriteBook) {
    console.log(`Invalid book: ${book}`);

    book = input.shift();
  }
  console.log("Book found!");
}
```
[/code-editor]
[task-description]
Write a function, which: 

* Receives a favorite book's name
* Receives books names until it gets the favorite book
* Prints:
    * "Book found!" and stops afterwards
    * "Invalid book: " + book for all invalid books
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|Alice in Wonderland|Book Found!|
|Winnie the Pooh||
|Alice in Wonderland||
[/slide]

[slide]
# Problem: Find Min and Max
[code-task title="Find Min and Max" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function minAndMax(input) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a function to find the min and max numbers

* Reads numbers until ***"END"*** is entered
* Prints the **biggest** and the **smallest** number

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10|Min number: 0|
|20|Max number: 304|
|304||
|0||
|50||
|END||
[/slide]

[slide]
# Solution: Find Min and Max
[code-task title="Find Min and Max" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function minAndMax(input) {
  let min = Number.MAX_SAFE_INTEGER;
  let max = Number.MIN_SAFE_INTEGER;
  let nextLine = input.shift();
  while (nextLine !== "END") {
    let num = Number(nextLine);
    if (num < min) { 
      min = num;
    }
    
    if (num > max) {
      max = num;
    }
    
    nextLine = lines.shift();
  }

  console.log(`Min number: ${min}`);
  console.log(`Max number: ${max}`);
}
```
[/code-editor]
[task-description]
Write a function to find the min and max numbers

* Reads numbers until ***"END"*** is entered
* Prints the **biggest** and the **smallest** number

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10|Min number: 0|
|20|Max number: 304|
|304||
|0||
|50||
|END||
[/slide]

[slide]
# Problem: Special Number
[code-task title="Special Number" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function specialNumber(input) {
  // Write your code here 
}
```
[/code-editor]
[task-description]
Write a function to check if given number is special: 

* Special numbers are divisible by all of their digits without remainder
* Receives a number and check whether it is a special number
* Print "\{num\} is special" if the number is special
* Otherwise, print "\{num\} is not special"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|23|23 is not special|
|204|204 is special|
[/slide]

[slide]
# Solution: Special Number
[code-task title="Special Number" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function specialNumber(input) {
  let num = Number(input.shift());
  let numDigits = num;
  let isSpecial = true;

  while (numDigits > 0) {
    let digit = numDigits % 10;
    numDigits /= 10;
    
    if (digit != 0 && num % digit != 0) {
      isSpecial = false;
      break;
    }
  }
  
  if (isSpecial) {
    console.log(`${num} is special)`;
  } else {
    console.log(`${num} is not special)`;
  }
}
```
[/code-editor]
[task-description]
Write a function to check if given number is special: 

* Special numbers are divisible by all of their digits without remainder
* Receives a number and check whether it is a special number
* Print "\{num\} is special" if the number is special
* Otherwise, print "\{num\} is not special"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|23|23 is not special|
|204|204 is special|
[/slide]

[slide]
# Problem: Special Bonus
[code-task title="Special Bonus" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function specialBonus(nums) {
  // Write your code here
}

```
[/code-editor]
[task-description]
Write a function to apply a **20% bonus** for certain number:

* Receives a numbers from the console: the "stop number"
* Receives numbers until it finds the stop number
* When the stop number is found, increase the value of the **previous** number **before it** with 20% and print it
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|25|36|
|20||
|30||
|25||
[/slide]

[slide]
# Solution: Special Bonus
[code-task title="Special Bonus" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function specialBonus(input) {
  let stopNum = Number(input.shift());
  let previousNum = stopNum;
  while (true) {
    let num = Number(input.shift());
    
    if (num === stopNum) {
      break;
    }
    
    previousNum = num;
  }
  
  console.log(previousNum * 1.2);
}
```
[/code-editor]
[task-description]
Write a function to apply a **20% bonus** for certain number:

* Receives a numbers from the console: the "stop number"
* Receives numbers until it finds the stop number
* When the stop number is found, increase the value of the **previous** number **before it** with 20% and print it
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|25|36|
|20||
|30||
|25||
[/slide]

[slide]
# Problem: Account Balance
[code-task title="Account Balance" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function accountBalance(input) {
  // Write your code here
}

```
[/code-editor]
[task-description]
Write a function to calculate an account balance 

* Receives a sequence of **incomes / expenses**, until "End" is read
* Adds the money to the balance (starting form 0) and print "Increase: \{money\} " or "Decrease: \{money\}"
* Finally, prints the account balance

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|500|Increase: 500.00|
|15.5|Increase: 15.50|
|80.35|Decrease: 80.35|
|END|Balance: 435.15|
[/slide]

[slide]
# Solution: Account Balance
[code-task title="Account Balance" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function accountBalance(lines) {
  let balance = 0;
  let input = lines.shift();
  
  while (input !== 'End') {
    let amount = Number(input);
    balance += amount;

    if (amount >= 0) {
      console.log(`Increase: ${amount.toFixed(2)}`);
    } else {
      console.log(`Decrease: ${amount.toFixed(2)}`);
    }
  }

  console.log(`Balance: ${balance.toFixed(2)}`);
}
```
[/code-editor]
[task-description]
Write a function to calculate an account balance 

* Receives a sequence of **incomes / expenses**, until "End" is read
* Adds the money to the balance (starting form 0) and print "Increase: \{money\} " or "Decrease: \{money\}"
* Finally, prints the account balance

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|500|Increase: 500.00|
|15.5|Increase: 15.50|
|80.35|Decrease: 80.35|
|END|Balance: 435.15|
[/slide]