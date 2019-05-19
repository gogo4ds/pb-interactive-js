[slide]
# What is Coding?
**Coding** means to give **commands** to tell the computer what to do

Sample command:
```js
console.log("I am coding");
```
A **computer program** is a sequence of commands
```js
console.log("First command");
console.log("Second command");
console.log("Third command");
```
[/slide]

[slide]
# Running JavaScript Commands
The easiest way to run JavaScript commands (JS commands)

The **browser console**: press \[F12\] in your Web browser

[image src="https://github.com/AlenPaunov/pb-interactive-js/blob/master/assets/intro-to-programming-1.png"/]
[/slide]

[slide]
# Commands in JavaScript – Examples 
Calculate an expression and print its value:
```js
console.log(5 + 5);
```
Calculate an area of rectangle:
```js
console.log(base * height / 2);
```
Print the numbers from 1 to 100
```js
for (let i = 1; i <= 100; i++)
    console.log(i);
```
[/slide]

[slide]
# Programming and Algorithms 
**Programming** means writing computer programs (commands)

* Using certain **programming language**, such as JavaScript or Python

**Algorithm** == a sequence of commands that achieves certain result

Programming is done by **programmers** (developers)

Programmers use IDE (like Visual Studio Code) to:

* **Write** the code
* **Run** and test the code
* Find a fix **bugs** (debug the code)
[/slide]

[slide]
# Computer Program – Example
Sample C# program (sequence of JavaScript commands):

```js
let size = 5;
console.log("Size = " + size);
console.log("Area = " + size * size);
```

[image src="https://github.com/AlenPaunov/pb-interactive-js/blob/master/assets/intro-to-programming-2.png"/]
[/slide]

[slide]
# Complete Computer Program
Sample complete JavaScript program (class + method + commands):
```js
function calculateArea() {
  let size = 5;
  console.log("Size = " + size);
  console.log("Area = " + size * size);
}
calculateArea();
```
[/slide]

[slide]
# Console-Based JavaScript Program – Example
JavaScript program, which converts from USD to EUR
```js
function convertUsdToEur(input) {
  let dollars = parseFloat(input);
  let euro = dollars * 0.883795087;
  console.log("Euro: " + euro);
}
convertUsdToEur("5");
```
[/slide]

[slide]
# Browser-Based JS Program – Example
Convert from **USD** to **EUR** in a Web page (HTML code)
```html
<html><body>
  <script src="converter.js"></script>
  Dollars: <input type="text" id="dollarsBox" />
  <button onclick="convertUsdToEur()">Convert</button>
  Euro: <input type="text" id="eurosBox" readonly />
</body></html>
```
```js
function convertUsdToEur() {
  let dollars = parseFloat(
    document.getElementById("dollarsBox").value);
  let euro = dollars * 0.883795087;
  document.getElementById("eurosBox").value = euro;
}
```
[/slide]