[slide]
# Complex Loops
Loops with different steps
```js
for (let i = n; i >= 1; i--) …
```
```js
for (let j = 1; j <= n; j+=2) …
```
```js
for (let k = 1; k <= n; k*=2) …
```
```js
for (let d = n; d > 0; d/=2) …
```
[/slide]

[slide]
# Problem: Numbers form N to 1
[code-task title="Numbers form N to 1" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function numbersFromNto1(n) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a function to print the numbers from N down to 1

* Receives a number **n**
* Prints the numbers from **n** down to **1**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10|10|
||9|
||8|
||7|
||6|
||5|
||4|
||3|
||2|
||1|
[/slide]

[slide]
# Solution: Numbers form N to 1
[code-task title="Numbers form N to 1" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function numbersWithStep(n) {
  let result = '';
  for (let i = 1; i <= n; i += 3) {
    if (i > 1)
      result += ", ";
    result += i;
  }
  console.log(result);
}
```
[/code-editor]
[task-description]
Write a function to print the numbers from N down to 1

* Receives a number **n**
* Prints the numbers from **n** down to **1**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10|10|
||9|
||8|
||7|
||6|
||5|
||4|
||3|
||2|
||1|
[/slide]

[slide]
# Problem: Even Powers of 2
[code-task title="Even Powers of 2" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function evenPowersOf2(n) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a function to print the even powers of 2:

* Receives a number n
* Prints the even powers of 2 up to 2n:
    * 20, 22, 24, 28, …, 2n
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|1|
||4|
||16|
[/slide]

[slide]
# Solution: Even Powers of 2
[code-task title="Even Powers of 2" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function evenPowersOf2(n) {
  let num = 1;
  let result = '';
  for (let i = 0; i <= n; i += 2) {
    if (i > 0)
      result += ", ";
    result += num;
    num = num * 2 * 2;
  }
  console.log(result);
}
```
[/code-editor]
[task-description]
Write a function to print the even powers of 2:

* Receives a number n
* Prints the even powers of 2 up to 2n:
    * 20, 22, 24, 28, …, 2n
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|1|
||4|
||16|
[/slide]