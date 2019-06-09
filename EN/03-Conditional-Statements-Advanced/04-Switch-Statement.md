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

[slide]
# Multiple Labels
Used when the same logic has to be executed in more than one case
```js
switch (selector) {
  case value1:
  case value2:
    statements;
    break;
  default:
    statements; 
    break;
}
```
# Example
```js
function printAnimalType(animal) {
   switch (animal) {
      case "dog":
      case "cat":
         console.log("mammal");
         break;
      default:
         console.log("unknown"); 
         break;
   }
}
```
[/slide]