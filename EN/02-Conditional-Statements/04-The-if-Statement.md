[slide]
# Simple Conditions
Check certain condition and take action according to the result
```js
if (condition) {
  // Code for execution if  
 // the condition is true
} 
```
The condition holds true or false
[/slide]

[slide]
# Problem: Freezing Weather
[code-task title="Freezing weather" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```js
function freezingWeather([temperature]) {
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
function freezingWeather([temperature]) {
    if (Number(temperature) <= 0) {
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
