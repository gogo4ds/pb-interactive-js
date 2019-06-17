[slide]
# Homework
Now, it's your turn to practice what you have learned in the training session.

We have prepared some simple problems for you to solve. If you struggle you can see the solution after each problem. 
[/slide]

[slide]
# Problem: Number Sequence
[code-task title="Number Sequence" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function numberSequence(input) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n representing the count of numbers to read next
* Finds the max and the min numbers
* Prints them on the console
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|Max number: 304|
|10|Min number: 0|
|304||
|0||
|0||
|50||
[/slide]

[slide]
# Solution: Number Sequence
[code-task title="Number Sequence" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function numberSequence(input) {
  let n = Number(input.shift());
  let min = Number.MAX_SAFE_INTEGER;
  let max = Number.MIN_SAFE_INTEGER;
  for (let i = 0; i < n; i++) {
      let num = Number(input.shift());
      if (num < min) min = num;
      if (num > max) max = num;
  }

  console.log(`Max number: ${max}`);
  console.log(`Min number: ${min}`);
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n representing the count of numbers to read next
* Finds the max and the min numbers
* Prints them on the console
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|Max number: 304|
|10|Min number: 0|
|304||
|0||
|0||
|50||
[/slide]

[slide]
# Problem: Power Of Numbers
[code-task title="Power Of Numbers" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function powerOfNumbers(input) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads p – the power and n – the number
* Prints the result of n powered by p
* Don't use Math.Pow()
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|32|
|2||
|4|81|
|3||
[/slide]

[slide]
# Solution: Power Of Numbers
[code-task title="Power Of Numbers" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function powerOfNumbers(input) {
  let p = Number(input.shift());
  let n = Number(input.shift());
  let result = 1;

  for(let i = 0; i < p; i++) {
    result = result * n;
  }

  console.log(result);
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads p – the power and n – the number
* Prints the result of n powered by p
* Don't use Math.Pow()
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|32|
|2||
|4|81|
|3||
[/slide]

[slide]
# Problem: Equal Pairs
[code-task title="Equal Pairs" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function equalPairs(input) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads number n and n pairs of numbers
* Prints "Yes, value={sum}", if the sum of all pairs is the same
* Otherwise, prints "No, maxdiff={diff}"
* diff is the max difference in the sum between two pairs
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|Yes, value=-1|
|-1||
|0||
|0||
|-1||
[/slide]

[slide]
# Solution: Equal Pairs
[code-task title="Equal Pairs" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function equalPairs(input) {
  let n = Number(input.shift());
  let prevSum = 0;
  let maxDiff = 0;
  let areEqual = true;
  
  for (let i = 0; i < n; i++) {
    let a = Number(input.shift());
    let b = Number(input.shift());

    if (i > 0) {
      if (maxDiff < Math.abs(prevSum - a - b)) {
        maxDiff = Math.abs(prevSum - a - b);
      }
      
      if (areEqual && a + b != prevSum) {
        areEqual = false;
      }
    }

    prevSum = a + b;
  }

  if (areEqual) {
    console.log(`Yes, value=${prevSum}`);
  } else {
    console.log(`No, maxdiff=${maxDiff}`);
  }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads number n and n pairs of numbers
* Prints "Yes, value={sum}", if the sum of all pairs is the same
* Otherwise, prints "No, maxdiff={diff}"
* diff is the max difference in the sum between two pairs
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|Yes, value=-1|
|-1||
|0||
|0||
|-1||
[/slide]

[slide]
# Problem: Bigger Number
[code-task title="Bigger Number" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function biggerNumber(input) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n - number representing amount of input numbers
* Reads n numbers
* Finds and prints the biggest number
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|90|
|40||
|90||
|50||
|3|-40|
|-40||
|-90||
|-50||
[/slide]

[slide]
# Solution: Bigger Number
[code-task title="Bigger Number" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function biggerNumber(input) {
  let n = Number(input.shift());
  let maxNumber = Number.MIN_SAFE_INTEGER;

  for (let i = 1; i <= n; i++) {
    let number = Number(input.shift());
    if (number > maxNumber) {
        maxNumber = number;
    }
  }
  
  console.log(maxNumber);
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n - number representing amount of input numbers
* Reads n numbers
* Finds and prints the biggest number
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|90|
|40||
|90||
|50||
|3|-40|
|-40||
|-90||
|-50||
[/slide]

[slide]
# Problem: Zig Zag Sum
[code-task title="Zig Zag Sum" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function zigZagSum(input) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n - number representing amount of input numbers
* Reads n numbers 
* For every even line adds the number to the result
* For every odd line subtracts the number from the result
* Prints the result
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|-30|
|10||
|20||
[/slide]

[slide]
# Solution: Zig Zag Sum
[code-task title="Zig Zag Sum" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function zigZagSum(input) {
  let n = Number(input.shift());
  let sum = 0;
  for (let i = 1; i <= n; i++) {
    let m = Number(input.shift());
    if (i % 2 == 0) sum += m;
    else sum -= m;
  }

  console.log(sum);
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n - number representing amount of input numbers
* Reads n numbers 
* For every even line adds the number to the result
* For every odd line subtracts the number from the result
* Prints the result
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|-30|
|10||
|20||
[/slide]

[slide]
# Problem: Divide Without Remainder
[code-task title="Divide Without Remainder" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function divideWithoutRemainder(input) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n and n numbers
* Finds in percentage how many of them can divide without remainder at 2, 3 and 4
* Prints percentages p1, p2 and p3, formatted to the second digit
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|33.33%|
|3|100.00%|
|6|0.00%|
|9||
[/slide]

[slide]
# Solution: Divide Without Remainder
[code-task title="Divide Without Remainder" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function divideWithoutRemainder(input) {
  let n = Number(input.shift());
  let p1 = 0.0;
  let p2 = 0.0;
  let p3 = 0.0;
  for (let i = 0; i < n; i++) {
    let num = Number(input.shift());
    if (num % 2 == 0) p1++;
    if (num % 3 == 0) p2++;
    if (num % 4 == 0) p3++;
  }

  let resultP1 = (p1 / n) * 100;
  let resultP2 = (p2 / n) * 100;
  let resultP3 = (p3 / n) * 100;
  
  console.log(`{resultP1.toFixed(2):F2}%`);
  console.log(`{resultP2.toFixed(2):F2}%`);
  console.log(`{resultP3.toFixed(2):F2}%`);
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n and n numbers
* Finds in percentage how many of them can divide without remainder at 2, 3 and 4
* Prints percentages p1, p2 and p3, formatted to the second digit
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|33.33%|
|3|100.00%|
|6|0.00%|
|9||
[/slide]

[slide]
# Problem: Vowel Sum
[code-task title="Vowel Sum" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function vowelSum(input) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n - the count of characters:
* If character is vowel adds its value to the result

    |character|a|e|i|o|u|
    |---------|-|-|-|-|-|
    |value|1|2|3|4|5|

* Prints the result
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|1|
|a||
|g||
|2|8|
|i||
|u||
[/slide]

[slide]
# Solution: Vowel Sum
[code-task title="Vowel Sum" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function vowelSum(input) {
  let n = Number(input.shift());
  let vowelSum = 0;
  for (let i = 0; i < n; i++) {
    let letter = input.shift();
    switch (letter) {
        case 'a':
          vowelSum += 1;
          break;
        case 'e':
          vowelSum += 2;
          break;
        case 'i':
          vowelSum += 3;
          break;
        case 'o':
          vowelSum += 4;
          break;
        case 'u':
          vowelSum += 5;
          break;
    }
  }
  console.log(vowelSum);
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n - the count of characters:
* If character is vowel adds its value to the result

    |character|a|e|i|o|u|
    |---------|-|-|-|-|-|
    |value|1|2|3|4|5|

* Prints the result
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2<br>a<br>g|1|
|a||
|g||
[/slide]

[slide]
# Problem: Rollercoaster
[code-task title="Rollercoaster" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function rollercoaster(input) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads rollercoaster places, minimum age, count of people on the queue and age for each person
* If all places are taken, prints - "The rollercoaster departures"
* In other case, prints "Waiting..."
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|1|
|a||
|g||
|2|8|
|i||
|u||
[/slide]

[slide]
# Solution: Rollercoaster
[code-task title="Rollercoaster" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function rollercoaster(input) {
  let rollercoasterPlaces = Number(input.shift());
  let minAge = Number(input.shift());
  let peopleCount = Number(input.shift());
  let validPeopleCount = 0;
  for (let i = 0; i < peopleCount; i++) {
    let personAge = Number(input.shift());
    if (personAge >= minAge && rollercoasterPlaces > validPeopleCount) {
        validPeopleCount++;
    }
  } 
  
  if (rollercoasterPlaces == validPeopleCount) {
    console.log("The rollercoaster departures");
  } else {
    console.log("Waiting...");
  }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads rollercoaster places, minimum age, count of people on the queue and age for each person
* If all places are taken, prints - "The rollercoaster departures"
* In other case, prints "Waiting..."
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|The rollercoaster departures|
|10||
|1||
|15||
[/slide]

[slide]
# Problem: Multiply
[code-task title="Multiply" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function multiply(input) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a program, which: 

* Reads n 
* Prints n's multiples in the format "{n} x {i} = {result}"
* Where i are the numbers from 1 to 10 (inclusive)
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|2 x 1 = 2|
||2 x 2 = 4|
||2 x 3 = 6|
||2 x 4 = 8|
||2 x 5 = 10|
||2 x 6 = 12|
||2 x 7 = 14|
||2 x 8 = 16|
||2 x 9 = 18|
||2 x 10 = 20|
[/slide]

[slide]
# Problem: Multiply
[code-task title="Multiply" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function multiply(input) {
  let n = Number(input.shift());
  for (let i = 1; i <= 10; i++) {
    let result = n * i;
    console.log(`${n} x ${i} = ${result}`);
  }
}
```
[/code-editor]
[task-description]
Write a program, which: 

* Reads n 
* Prints n's multiples in the format "{n} x {i} = {result}"
* Where i are the numbers from 1 to 10 (inclusive)
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|2 x 1 = 2|
||2 x 2 = 4|
||2 x 3 = 6|
||2 x 4 = 8|
||2 x 5 = 10|
||2 x 6 = 12|
||2 x 7 = 14|
||2 x 8 = 16|
||2 x 9 = 18|
||2 x 10 = 20|
[/slide]