[slide]
# Homework
Now, it's your turn to practice what you have learned in the training session.

We have prepared some simple problems for you to solve. If you struggle you can see the solution after each problem. 
[/slide]

[slide]
# Problem: Guess the Password
[code-task title="Guess the Password" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```js
function guessThePassword(input) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which: 
* Receives a string that is a **password**
* Prints "**Welcome**" if the password is "**s3cr3t!**"
* Prints "**Wrong password!**" in all other cases 
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|s3cr3t!|Welcome|
|qwerty|Wrong password!|
[/slide]

[slide]
# Solution: Guess the Password
[code-task title="Guess the Password" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```js
function guessThePassword(input) {
  let password = input.shift();
  if (password == "s3cr3t!") {
    console.log("Welcome");
  } else {
    console.log("Wrong password!");
  }
}
```
[/code-editor]
[task-description]
Write a function, which: 
* Receives a string that is a **password**
* Prints "**Welcome**" if the password is "**s3cr3t!**"
* Prints "**Wrong password!**" in all other cases 
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|s3cr3t!|Welcome|
|qwerty|Wrong password!|
[/slide]

[slide]
# Problem: Boiling Water
[code-task title="Boiling Water" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```js
function boilingWater(input) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which: 
* Receives a **single parameter**: the water temperature (in °C)
* Prints "**The water is boiling**" if the number > 100
* Prints "**The water is not hot enough**" in all other cases
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|104.8|The water is boiling|
|29|The water is not hot enough|
[/slide]

[slide]
# Solution: Boiling Water
[code-task title="Boiling Water" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```js
function boilingWater(input) {
  let degrees = Number(input.shift());
  if (degrees > 100) {
    console.log("The water is boiling"); 
  } else {
    console.log("The water is not hot enough");
  }
}
```
[/code-editor]
[task-description]
Write a function, which: 
* Receives a **single parameter**: the water temperature (in °C)
* Prints "**The water is boiling**" if the number > 100
* Prints "**The water is not hot enough**" in all other cases
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|104.8|The water is boiling|
|29|The water is not hot enough|
[/slide]

[slide]
# Problem: Speed Info
[code-task title="Speed Info" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```js
function speedInfo(input) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which: 
* Receives a single parameter (**speed**)
* Prints "**Slow**" if the number **<=** 30
* Prints "**Fast**" if the number **>** 30
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|30|Slow|
|60|Fast|
[/slide]

[slide]
# Solution: Speed Info
[code-task title="Speed Info" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```js
function speedInfo(input) {
  let speed = Number(input.shift());
  if (speed <= 30) {
    console.log("Slow");
  } else {
    console.log("Fast");
  }
}
```
[/code-editor]
[task-description]
Write a function, which: 
* Receives a single parameter (**speed**)
* Prints "**Slow**" if the number **<=** 30
* Prints "**Fast**" if the number **>** 30
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|30|Slow|
|60|Fast|
[/slide]

[slide]
# Problem: Area of Figures
[code-task title="Area of Figures" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```js
function areaOfFigures(input) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which: 
* Receives a type of figure and its side
* Checks if the figure is **square** or **circle**
* Prints the calculated area **formatted** to the **second decimal**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|square|25.00|
|5||
[/slide]

[slide]
# Solution: Area of Figures
[code-task title="Area of Figures" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```js
function areaOfFigures(input) {
  let figure = Number(input.shift());
  let side = Number(input.shift());
  let area = 0;
  if (figure === 'square') {
    area = Number(side) * Number(side)
  } else {
    area = Math.PI * Number(side) * Number(side)
  }
  console.log(`${area.toFixed(2)}`);
}
```
[/code-editor]
[task-description]
Write a function, which: 
* Receives a type of figure and its side
* Checks if the figure is **square** or **circle**
* Prints the calculated area **formatted** to the **second decimal**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|square|25.00|
|5||
[/slide]

[slide]
# Problem: Tickets
[code-task title="Tickets" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```js
function tickets(input) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which: 
* Receives a **ticket type** - either "**student**" or "**regular**"
* Prints the price in the following format: "$\{price\}" 
    * Student ticket is 1.60
    * Regular ticket is 1.00
    * For invalid type "**Invalid ticket type!**"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|student|$1.00|
|regular|$1.60|
[/slide]


[slide]
# Solution: Tickets
[code-task title="Tickets" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```js
function tickets(input) {
  let ticketType = input.shift();
  if (ticketType === 'student') {
    console.log('$1.00');
  } else if (ticketType === 'regular') {
    console.log('$1.60');
  } else {
    console.log('Invalid ticket type!');
  }
}
```
[/code-editor]
[task-description]
Write a function, which: 
* Receives a **ticket type** - either "**student**" or "**regular**"
* Prints the price in the following format: "$\{price\}" 
    * Student ticket is 1.60
    * Regular ticket is 1.00
    * For invalid type "**Invalid ticket type!**"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|student|$1.00|
|regular|$1.60|
[/slide]

[slide]
# Problem: Coffee Shop
[code-task title="Coffee Shop" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```js
function coffeeShop(input) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which: 
* Receives a drink - either "**coffee**" or "**tea**"
* Receives an **extra** - either "**sugar**" or "**no**"
* Prints a price in format "Final price: \{price\}"
Prices
* Coffee - 1.00
* Tea - 0.60
* Sugar - 0.40
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|coffee|1.4|
|sugar||

|Input|Output|
|-----|------|
|tea|0.6|
|no||
[/slide]

[slide]
# Solution: Coffee Shop
[code-task title="Coffee Shop" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```js
function coffeeShop(input) {
  let order = input.shift(); 
  let extra = input.shift();
  let price = 0;
  if (order === 'coffee')
    price = 1.00
  else if (order === 'tea')
    price = 0.60
  if (extra === 'sugar')
    price += 0.40
  console.log(`Final price: ${price}`);
}
```
[/code-editor]
[task-description]
Write a function, which: 
* Receives a drink - either "**coffee**" or "**tea**"
* Receives an **extra** - either "**sugar**" or "**no**"
* Prints a price in format "Final price: \{price\}"
Prices
* Coffee - 1.00
* Tea - 0.60
* Sugar - 0.40
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|coffee|1.4|
|sugar||

|Input|Output|
|-----|------|
|tea|0.6|
|no||
[/slide]

[slide]
# Problem: Valid Triangle
[code-task title="Valid Triangle" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```js
function validTriangle(input) {
    // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which: 
* Receives **3 arguments** - the **sides** of a **triangle**
* Checks if each **side** is **lesser** than the **sum** of the **other 2**
* Prints "**Valid Triangle**" if the above condition is met
* Prints "**Invalid Triangle**" otherwise 
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|Valid Triangle|
|4||
|5||
[/slide]

[slide]
# Solution: Valid Triangle
[code-task title="Valid Triangle" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```js
function validTriangle(input) {
  let a = Number(input.shift());
  let b = Number(input.shift());
  let c = Number(input.shift());
  let isValidTriangle = true;
  if (a + b <= c) {
    isValidTriangle = false;
  } else if (a + c <= b) {
    isValidTriangle = false;
  } else if (b + c <= a) {
    isValidTriangle = false;
  }

  if (isValidTriangle) {
    console.log("Valid Triangle");
  } else {
    console.log("Invalid Trianlge");
  }
}
```
[/code-editor]
[task-description]
Write a function, which: 
* Receives **3 arguments** - the **sides** of a **triangle**
* Checks if each **side** is **lesser** than the **sum** of the **other 2**
* Prints "**Valid Triangle**" if the above condition is met
* Prints "**Invalid Triangle**" otherwise 
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|Valid Triangle|
|4||
|5||
[/slide]
