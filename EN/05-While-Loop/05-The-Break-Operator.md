[slide]
# The "break" Operator
Used for prematurely **exiting** the loop

Can only be executed from the loop's **body**

When break is executed, the code inside the loop's body after it **is skipped** (does not execute)

Example:
```js
function solve(nums) {
  while (true) {
    let num = Number(nums.shift());
    if (num % 2 !== 0) {
      // Odd number is entered
      break;
    }
    console.log("Enter an odd number!");
  }
  console.log("Odd number: " + num);
}
```
[/slide]