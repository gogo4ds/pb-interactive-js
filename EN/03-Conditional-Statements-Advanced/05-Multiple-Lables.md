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