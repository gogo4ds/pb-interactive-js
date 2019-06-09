[slide]
# Switch
The switch statement evaluates an expression, matching the expression's value to a case clause

Alternative to an **if-else** statement

```
switch (selector) {
    case value1:
      statements;
      break;
    case value2:
      statements;
      break;
}
```

# Default Clause
The default clause is executed if the value of expression doesn't match any of the case clauses

```
switch (selector) {
    case value1:
      statements;
      break;
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
Used when the same logic has to be executed for different cases

```
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
function animalType(animal) {
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