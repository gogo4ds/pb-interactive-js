[slide]
# While Loop
Control flow **statement**

* Executes code repeatedly while a condition is true
```js
while (condition) {
   // Body of the loop
}
```
Example: Print numbers from **1 to 5**
```js
let i = 1;
while (i <= 5) {
   console.log(i);
   i++;
}
```
[/slide]

[slide]
# While or For?
***while*** and ***for*** loops **repeat** blocks of **code**

Use ***for*** when you know in advance the **number of repetitions**

Use ***while*** when you don't know when the **exit condition** will be met
[/slide]

[slide]
# The "break" Operator
Used for **prematurely exiting** the loop

Can only be executed from the **body**, during **an iteration** of the loop

***break*** immediately exits from the loop

* The rest of the loop body **is skipped**
```js
let i = 1;
while (true) {
  if (i>10) break;
  i++;
}
```
[/slide]