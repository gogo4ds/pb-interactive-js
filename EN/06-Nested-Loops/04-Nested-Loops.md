[slide]
# Nested Loops
We can nest a **loop inside another loop**:
```js
let n = 3;
let rowLine = '';
for (let row = 1; row <= n; row++) {
  for (let col = 1; col <= n; col++) {
    rowLine += ' *';
  }
  rowLine += '\n';
}
console.log(rowLine);
```
[/slide]

[slide]
# Nested Loops
Nested loops == several **loops** located **inside each other**
**Nested loops** are used:
* To execute multiple times an **action**, which **executes** multiple **actions**
* To implement more **complex** calculations and program logic
[/slide]

[slide]
# Multiple Levels of Nested Loops
```js
for (let i = 1; i <= n; i += 3) {
  for (let j = 1; j <= n; j += 3) {
    for (let k = 1; k <= n; k += 3) {
      // ...
    }
  }
}
```
The loop variable names must be different
[/slide]