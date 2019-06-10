[slide]
# Revision

# The if Statement
Very often you want to perform different actions for different conditions

The if statement executes a statement if a specified condition is true

```js
function greet (hour) {
  if (hour < 18) {
     console.log("Good day");
  }
}

greet(10);   // Good day
greet(19);   // No output
```

# The else Statement
If the condition is false, another statement can be executed

```js
function greet (hour) {
  if (hour < 18) {
     console.log("Good day");
  } else {
     console.log("Good evening");
  }
}

greet(19); // Good evening
```

# The else-if Statement
Used to chain multiple checks

```js
function greet (hour) {
  if (hour < 10) {
     console.log("Good morning");
  } else if (hour < 18) {
     console.log("Good day");
  } else {
     console.log("Good evening");
  }
}
```
[/slide]