[slide]
# If Statement
One of the single most important statements in every programming language is the if statement

The if statement needs a boolean result, that is, true or false
  * If the boolean result is true take action 

```js
if (condition) {
  // Code for execution if the condition is true
} 
```
[/slide]

[slide]
# Problem: Freezing Weather
[code-task title="Freezing weather" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```js
function freezingWeather(input) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which:
* Receives a temperature in Celsius
* **Checks** whether the temperature is **below** zero
* Prints "**Freezing weather!**", if the temperature is equal or smaller than 0
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|4|(No output)|
|-2|Freezing weather!|
[/slide]

[slide]
# Solution: Freezing Weather
[code-task title="Freezing weather" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```js
function freezingWeather(input) {
  let temperature = Number(input.shift());
  if (temperature <= 0) {
    console.log("Freezing weather!");
  }
}
```
[/code-editor]
[task-description]
Write a function, which:
* Receives a temperature in Celsius
* **Checks** whether the temperature is **below** zero
* Prints "**Freezing weather!**", if the temperature is equal or smaller than 0
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|4|(No output)|
|-2|Freezing weather!|
[/slide]
