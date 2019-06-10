[slide]
# Real Life Example
Each day of our lives is an **iteration** in a for loop

[image src="https://github.com/AlenPaunov/pb-interactive-course/blob/04-js-for-loops/assets/for-loops-1.png"/]
[/slide]

[slide]
# For Loop
Allows code to be executed **repeatedly**

Repeating while the condition is met
```js
for (initialization; condition; step) {
    // Body of the for loop
}
```
**Initialization** - initializes the variable

**Condition** - evaluates the condition

**Step** - updates the initialized value

# Example
```js
for (let i = 1; i <= 10; i += 1) {
  console.log(i);
}
```
[/slide]

[slide]
# Problem: Print Sum of N Numbers
[code-task title="Print Sum of N Numbers" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function printSum (n) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a number n
* Sums all numbers from 1 to n
* Prints the sum on the console
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|15|
|6|21|
[/slide]

[slide]
# Solution: Print Sum of N Numbers
[code-task title="Print Sum of N Numbers" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function printSum (n) {
   let sum = 0;
   for (let i = 1; i <= n; i += 1) {
      sum += i;
   }
   console.log(sum);

}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a number n
* Sums all numbers from 1 to n
* Prints the sum on the console
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|15|
|6|21|
[/slide]

[slide]
# Problem: Calculate Month Salary
[code-task title="Calculate Month Salary" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function calculateMonthSalary (days, salaryPerDay) {
   // Write your code here
}

```
[/code-editor]
[task-description]
Write a function, which:

* Receives days in the current month and salary per day
* Calculates the salary for the month
* Prints the result on the console
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|30|300|
|10||
|28|560|
|20||
[/slide]

[slide]
# Problem: Calculate Month Salary
[code-task title="Calculate Month Salary" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function calculateMonthSalary (days, salaryPerDay) {
   let totalSalary = 0;
   for (int i = 1; i <= days; i += 1) {
      totalSalary += salaryPerDay;
   }
   console.log(totalSalary);

}

```
[/code-editor]
[task-description]
Write a function, which:

* Receives days in the current month and salary per day
* Calculates the salary for the month
* Prints the result on the console
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|30|300|
|10||
|28|560|
|20||
[/slide]