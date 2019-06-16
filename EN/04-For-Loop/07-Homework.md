[slide]
# Homework
Now, it's your turn to practice what you have learned in the training session.

We have prepared some simple problems for you to solve. If you struggle you can see the solution after each problem. 
[/slide]

[slide]
# Problem: Even Numbers n-m
[code-task title="Even Numbers n-m" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function evenNumbers (input) {
   // Write your code here
} 
```
[/code-editor]
[task-description]
Write a function, which:

* Receives two numbers: n and m
* Prints only the even numbers from n to m
* The number m will always be greater than n
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|2|
|6|4|
||6|
[/slide]

[slide]
# Solution: Even Numbers n-m
[code-task title="Even Numbers n-m" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function evenNumbers (input) {
   let n = Number(input.shift());
   let m = Number(input.shift());

   for (let i = n; i <= m; i++) {
      if (i % 2 === 0) {
         console.log(i);
      }
   }
}  
```
[/code-editor]
[task-description]
Write a function, which:

* Receives two numbers: n and m
* Prints only the even numbers from n to m
* The number m will always be greater than n
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|2|
|6|4|
||6|
[/slide]

[slide]
# Problem: Power of Numbers
[code-task title="Power of Numbers" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function powerOfNumber (input) {
   // Write your code here
}
 
```
[/code-editor]
[task-description]
Write a function, which:

* Receives p – the power and n – the number
* Prints the result of n powered by p

Don't use Math.pow()
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|32|
|2||
|4|81|
|3||
[/slide]

[slide]
# Solution: Power of Numbers
[code-task title="Power of Numbers" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function powerOfNumber (input) {
   let p = Number(input.shift());
   let n = Number(input.shift());

   let result = 1;
   for(let i = 0; i < p; i++) {
      result = result * n;
   }
   console.log(result);
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives p – the power and n – the number
* Prints the result of n powered by p

Don't use Math.pow()
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|32|
|2||
|4|81|
|3||
[/slide]

[slide]
# Problem: Multiply
[code-task title="Multiply" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function multiply (input) {
   // Write your code here
}
```
[/code-editor]
[task-description]
Write a program, which: 

* Reads n 
* Prints n's multiples in the format "\{n\} x \{i\} = \{result\}"
    * Where i are the numbers from 1 to 10 (inclusive)
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|2 x 1 = 2|
||2 x 2 = 4|
||2 x 3 = 6|
||2 x 4 = 8|
||2 x 5 = 10|
||2 x 6 = 12|
||2 x 7 = 14|
||2 x 8 = 16|
||2 x 9 = 18|
||2 x 10 = 20|
[/slide]

[slide]
# Solution: Multiply
[code-task title="Multiply" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function multiply (input) {
   let n = Number(input.shift());

   for(let i = 1; i <= 10; i++) {
      let result = n * i;
      console.log(`${n} x ${i} = ${result}`);
   }
}
```
[/code-editor]
[task-description]
Write a program, which: 

* Reads n 
* Prints n's multiples in the format "\{n\} x \{i\} = \{result\}"
    * Where i are the numbers from 1 to 10 (inclusive)
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|2 x 1 = 2|
||2 x 2 = 4|
||2 x 3 = 6|
||2 x 4 = 8|
||2 x 5 = 10|
||2 x 6 = 12|
||2 x 7 = 14|
||2 x 8 = 16|
||2 x 9 = 18|
||2 x 10 = 20|
[/slide]

[slide]
# Problem: Water Flowers
[code-task title="Water Flowers" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function waterFlowers (input) {
   // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives two numbers: weeks and step (condition for watering)
* Each \{step\} week you should water the flowers
* Print how many times you watered the flowers
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10|5|
|2||
[/slide]

[slide]
# Solution: Water Flowers
[code-task title="Water Flowers" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function waterFlowers (input) {
   let weeks = Number(input.shift());
   let step = Number(input.shift());

   let total = 0;
   for (let i = 1; i <= weeks; i++) {
      if (i % step === 0) {
         total++;
      }
   }
   console.log(total);
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives two numbers: weeks and step (condition for watering)
* Each \{step\} week you should water the flowers
* Print how many times you watered the flowers
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10|5|
|2||
[/slide]
