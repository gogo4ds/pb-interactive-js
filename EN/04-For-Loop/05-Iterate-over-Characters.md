[slide]
# ASCII Table

Computers can only understand numbers

* ASCII code is the numerical representation of a character

|Dec|Hx|Oct|Html|Chr|
|---|--|---|----|---|
|97|61|141|\&\#97;|a|
|98|62|142|\&\#98;|b|

* 'a' has the int value of 97
[/slide]

[slide]
# Character Conversions
Convert an ASCII / Unicode number into a character:
```js
let letter = String.fromCharCode(65);
console.log(letter); // A
```

Convert a character to its ASCII / Unicode code:
```js
let letter = 'A';
let asciiValue = letter.charCodeAt(0);
console.log(asciiValue); // 65
```
[/slide]

[slide]
# Iterating over Characters

We can iterate over characters using this code:

```js
for (let i = 65; i <= 90; i++) {
  let letter = String.fromCharCode(i);
  console.log(letter);
}

```

[/slide]

[slide]
# Problem: Latin Letters

[code-task title="Latin Letters" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function latinLetters(input) {
    // Write your code here...
}

```
[/code-editor]
[task-description]
Write a program, which:

* Reads 2 letters
* Prints all letters in the given range inclusive
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|ac|a b c|
|c||
|fl|f g h i g k l|
|l||
[/slide]

[slide]
# Solution: Latin Letters
[code-task title="Latin Letters" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function latinLetters(input) {
  let startChar = input.shift();
  let endChar = input.shift();
  
  let startValue = startChar.charCodeAt(0);
  let endValue = endChar.charCodeAt(0);
  let result = '';
  for (let i = startValue; i <= endValue; i++) {
    result += String.fromCharCode(i) + ' ';
  }
  console.log(result);
}

```
[/code-editor]
[task-description]
Write a program, which:

* Reads 2 letters
* Prints all letters in the given range inclusive
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|a|a b c|
|c||
|f|f g h i g k l|
|l||
[/slide]