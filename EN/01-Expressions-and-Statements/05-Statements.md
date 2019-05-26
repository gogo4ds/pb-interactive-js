[slide]
# Declaration Statements
***var*** - declares a variable, optionally initializing it to a value

***let*** - declares a block scope local variable, optionally initializing it to a value

***const*** - declares a read-only named constant

# Example
```js
const name = "Peter";
name = "John"; // this will not work
function sayHello () {
   let age = 25;
   console.log(name + " is " + age);
}
console.log(age);  // undefined
```
[/slide]