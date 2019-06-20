[slide]
# Problem: Sum of Digits Calculator
[code-task title="Sum of Digits Calculator" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function sumOfDigits(inputLines) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which: 
* Continuously **reads numbers** until "**End**" is entered
* Prints the sum of digits for each number
* Finally, prints "**Goodbye**"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|157|Sum of digits = 13|
|99|Sum of digits = 18|
|5|Sum of digits = 5|
|438|Sum of digits = 15|
|End|Goodbye|
[/slide]

[slide]
# Solution: Sum of Digits Calculator
[code-task title="Sum of Digits Calculator" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function sumOfDigits(inputLines) {
  while (true) {
    let input = inputLines.shift();
    if (input === "End") break;
    let sum = 0;
    for (let num = Number(input);
      num > 0; num = Math.floor(num / 10))
      sum += num % 10;
    console.log(`Sum of digits: ${sum}`);
  }
  console.log("Goodbye");
}
```
[/code-editor]
[task-description]
Write a function, which: 
* Continuously **reads numbers** until "**End**" is entered
* Prints the sum of digits for each number
* Finally, prints "**Goodbye**"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|157|Sum of digits = 13|
|99|Sum of digits = 18|
|5|Sum of digits = 5|
|438|Sum of digits = 15|
|End|Goodbye|
[/slide]