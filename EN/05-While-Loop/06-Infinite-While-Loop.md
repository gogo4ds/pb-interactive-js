[slide]
# Infinite While Loop
Infinite loop = repeating a block of code **an infinite number** of times

Infinite ***while*** loops: use ***true*** as loop condition

```js
while(true) {
    // Commands
}
```
[/slide]

[slide]
# Examples
```js
function infiniteWhileLoop(commands) {
  let command = "Add";
  
  while (command !== "End") { // Always true (never changed)
    console.log("Executing: " + command);
  }
}
```
```js
function infiniteWhileLoop(commands) {
  let command = "Add";
  
  while (command !== "End") {
    console.log("Executing: " + command);
    
    command = commands.shift();
  }
}
```
[/slide]