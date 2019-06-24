[slide]
# While of For
***while*** and ***fo***r loops both **repeat** a block of **code**

Use ***for***-loop when you preliminary know the **number of iterations**

Use ***while*** when you don't know when the exit condition will be met
[/slide]

[slide]
# Problem: Odd Number
[code-task title="Odd Number" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function oddNumber(numbers) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a program to enter an odd number

* Receives numbers from the console until an **odd number** is entered
* Print the **odd** number as output
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|3|
|4||
|8||
|3||
|5|5|
[/slide]

[slide]
# Solution: Odd Number
[code-task title="Odd Number" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function oddNumber(numbers) {
  let num = Number(numbers.shift());
  while (num % 2 === 0) {
    num = Number(numbers.shift());
  }
  console.log(num);
}
```
[/code-editor]
[task-description]
Write a program to enter an odd number

* Receives numbers from the console until an **odd number** is entered
* Print the **odd** number as output
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|3|
|4||
|8||
|3||
|5|5|
[/slide]

[slide]
# Problem: Number Processor
[code-task title="Number Processor" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function numberProcessor(input) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a function to process a sequence of commands:

* Receives a number from the console
* Receives a sequence of the following commands:
    * ***Add*** – adds 1 to the number
    * ***Subtract*** – subtracts 1 from the number
    * ***End*** – prints the number and stop the program
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|6|
|Add||
|End||
|5|4|
|Subtract||
|End||
[/slide]

[slide]
# Solution: Number Processor
[code-task title="Number Processor" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function numberProcessor(input) {
  let num = Number(input.shift());
  let command = input.shift();
  
  while (command !== "End") {
    switch (command) {
      case "Add": 
        num++; 
        break;
      case "Subtract": 
        num--; 
        break;
    }

    command = input.shift();
  }
  console.log(num);
}
```
[/code-editor]
[task-description]
Write a function to process a sequence of commands:

* Receives a number from the console
* Receives a sequence of the following commands:
    * ***Add*** – adds 1 to the number
    * ***Subtract*** – subtracts 1 from the number
    * ***End*** – prints the number and stop the program
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|6|
|Add||
|End||
|5|4|
|Subtract||
|End||
[/slide]