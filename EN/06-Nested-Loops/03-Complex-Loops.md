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
function numbersFromNto1(input) {
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
function numbersWithStep(input) {
  let n = Number(input.shift());
  let result = '';

  for (let i = n; i >= 1; i--) {
      console.log(result);
  }
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