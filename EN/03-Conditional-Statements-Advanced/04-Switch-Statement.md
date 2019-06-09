[slide]
# Switch
Used for choosing among a list of possibilities

Alternative to an **if-else** statement
```js
switch (selector) {
  case value1:
    statements;
    break;
  default:
    statements;
    break;
}
```
# Example
```js
function printResponse(choice) {
  switch (choice) {
    case "Y":
      console.log("Yes");
      break;
    case "N":
      console.log("No");
      break;
    default:
      console.log("Invalid response");
      break;
   }
}
```
[/slide]