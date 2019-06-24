[slide]
# Homework
Now, it's your turn to practice what you have learned in the training session.

We have prepared some simple problems for you to solve. If you struggle you can see the solution after each problem. 
[/slide]

[slide]
# Problem: Building
[code-task title="Building" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function building(floors, rooms) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a function to **print a table**, representing a **building**:
* Odd floors hold **apartments** (type **A**), e.g. **A10**, **A11**, **A12**, …
* Even floors hold **offices** (type **O**), e.g. **O20**, **O21**, **O22**, …
* The **last floor** holds large apartments (type **L**), e.g. **L60**, **L61**, **L62**
* Identifiers consist of: \{type\}\{floor\}\{number\}, e.g. **L65**, **A12**, **O24**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|6|L60 L61 L62 L63|
|4|A50 A51 A52 A53|
||O40 O41 O42 O43|
||A30 A31 A32 A33|
||O20 O21 O22 O23|
||A10 A11 A12 A13|
[/slide]

[slide]
# Solution: Building
[code-task title="Building" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function building(floors, rooms) {
  for (let f = floors; f >= 1; f--) {
    for (let r = 0; r < rooms; r++)
      if (f === floors) // Print last floor: L{f}{r}
      else if (f % 2 === 0) // Print office: O{f}{r}
      else // Print apartment: A{f}{r}
  }
}
```
[/code-editor]
[task-description]
Write a function to **print a table**, representing a **building**:
* Odd floors hold **apartments** (type **A**), e.g. **A10**, **A11**, **A12**, …
* Even floors hold **offices** (type **O**), e.g. **O20**, **O21**, **O22**, …
* The **last floor** holds large apartments (type **L**), e.g. **L60**, **L61**, **L62**
* Identifiers consist of: \{type\}\{floor\}\{number\}, e.g. **L65**, **A12**, **O24**
* Example: 
```js
L60 L61 L62 L63 L64 L65
A30 A31 A32 A33 A34 A35
O20 O21 O22 O23 O24 O25
A10 A11 A12 A13 A14 A15
```
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|6|L60 L61 L62 L63|
|4|A50 A51 A52 A53|
||O40 O41 O42 O43|
||A30 A31 A32 A33|
||O20 O21 O22 O23|
||A10 A11 A12 A13|
[/slide]

[slide]
# Problem: Stupid Passwords
[code-task title="Stupid Passwords" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function stupidPasswords(n) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a program, which **generates all possible passwords**, consisting of the following 3 parts:
* The **first** part is an **even** number in the range \[2…n\]
* The **second** digit is an **odd** number in the range \[1…n\]
* The **third** is the **product** of the first two
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|11|212 236 2510 2714 2918 21122 414 4312 4520 4728 4936 41144 616 6318 6530 6742 6954 61166 818 8324 8540 8756 8972 81188 10110 10330 10550 10770 10990 1011110|
|5|212 236 2510 414 4312 4520|
|6|212 236 2510 414 4312 4520 616 6318 6530|
[/slide]

[slide]
# Problem: Stupid Passwords
[code-task title="Stupid Passwords" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function stupidPasswords(n) {
  let result = '';
  for (let even = 2; even <= n; even += 2) {
    for (let odd = 1; odd <= n; odd += 2) {
      result += `${even}${odd}${even*odd} `;
    }
  }
  console.log(result);
}
```
[/code-editor]
[task-description]
Write a program, which **generates all possible passwords**, consisting of the following 3 parts:
* The **first** part is an **even** number in the range \[2…n\]
* The **second** digit is an **odd** number in the range \[1…n\]
* The **third** is the **product** of the first two
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|11|212 236 2510 2714 2918 21122 414 4312 4520 4728 4936 41144 616 6318 6530 6742 6954 61166 818 8324 8540 8756 8972 81188 10110 10330 10550 10770 10990 1011110|
|5|212 236 2510 414 4312 4520|
|6|212 236 2510 414 4312 4520 616 6318 6530|
[/slide]

[slide]
# Problem: Magic Numbers
[code-task title="Magic Numbers" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function magicNumbers(n) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a function to find all **3-digit magic numbers** of order **n**
* A number is **magic of order n** if the product of its digits is **n**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|111|
|3|113|
||131|
||311|
[/slide]

[slide]
# Solution: Magic Numbers
[code-task title="Magic Numbers" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function magicNumbers(n) {
  for (let d1 = 1; d1 <= 9; d1++)
    for (let d2 = 0; d2 <= 9; d2++)
      for (let d3 = 0; d3 <= 9; d3++)
        if (d1 * d2 * d3 === n)
          // TODO: Print {d1}{d2}{d3}
}
```
[/code-editor]
[task-description]
Write a function to find all **3-digit magic numbers** of order **n**
* A number is **magic of order n** if the product of its digits is **n**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|111|
|3|113|
||131|
||311|
[/slide]

[slide]
# Problem: Travelling
[code-task title="Travelling" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function travelling(inputLines) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which calculates the **money collection** for multiple travel destinations. It:
* Reads **destination** and **needed budget** for destination
* Reads many times amounts of collected money, until they are **enough** for the destination
* Prints "Collected: \{sum\}" or "Going to \{destination\}"
* Reads another destination and budget and collect money again
* Ends the program when a destination "**End**" is received
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|Bali|Collected: 800|
|3500|Collected: 2600|
|800|Collected: 3600|
|1800|Going to Bali!|
|1000|Collected: 5000|
|Brazil|Going to Brazil!|
|4600||
|5000||
|End||
[/slide]

[slide]
# Solution: Travelling
[code-task title="Travelling" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function travelling(inputLines) {
  let destination;
  while ((destination = inputLines.shift()) != "End") {
    let neededSum = Number(inputLines);
    let collectedSum = 0;
    while (collectedSum < neededSum) {
      collectedSum += Number(inputLines.shift());
      console.log(`Collected: ${collectedSum}`);
    }
    console.log(`Going to ${destination}!`);
  }
}
```
[/code-editor]
[task-description]
Write a function, which calculates the **money collection** for multiple travel destinations. It:
* Reads **destination** and **needed budget** for destination
* Reads many times amounts of collected money, until they are **enough** for the destination
* Prints "Collected: \{sum\}" or "Going to \{destination\}"
* Reads another destination and budget and collect money again
* Ends the program when a destination "**End**" is received
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|Bali|Collected: 800|
|3500|Collected: 2600|
|800|Collected: 3600|
|1800|Going to Bali!|
|1000|Collected: 5000|
|Brazil|Going to Brazil!|
|4600||
|5000||
|End||
[/slide]

[slide]
# Problem: Prime Numbers
[code-task title="Prime Numbers" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function primeNumbers(start, end) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a function to print all **prime numbers in a given range**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|5 7 11 13 17 19 23 29 31 37 41 43 47|
|50||
|20|23 29|
|30||
[/slide]

[slide]
# Solution: Prime Numbers
[code-task title="Prime Numbers" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function primeNumbers(start, end) {
  for (let num = start; num <= end; num++) {
    let prime = true;
    let divider = 2;
    let maxDivider = Math.floor(Math.sqrt(num));
    while (divider <= maxDivider) {
      if (num % divider == 0) {
        prime = false;
        break;
      }
      divider++;
    }
    if (prime) console.log(num);
  }
}
```
[/code-editor]
[task-description]
Write a function to print all **prime numbers in a given range**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|5 7 11 13 17 19 23 29 31 37 41 43 47|
|50||
|20|23 29|
|30||
[/slide]

[slide]
# Problem: Unique PIN Codes
[code-task title="Unique PIN Codes" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function pinCodes(max1, max2, max3) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a function to **generate PIN codes** following certain rules. It: 
* Receives **3 digits**: **max1**, **max2**, **max3** (each is an upper limit)
* Generates unique 3-digit **PIN codes**, matching the following:
    * Each digit is **within its range**: \[1..max1\], \[1..max2\], \[1..max3\]
    * The **first** and the **third digit** must be **even**
    * The **second digit** must be a **prime number** in the range \[2…7\]
* Prints the PIN codes in increasing order
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|222|
|5|224|
|5|232|
||234|
||252|
||254|
[/slide]

[slide]
# Solution: Unique PIN Codes
[code-task title="Unique PIN Codes" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function pinCodes(max1, max2, max3) {
  for (let d1 = 2; d1 <= max1; d1 += 2)
    for (let d2 = 2; d2 <= max2; d2++)
      for (let d3 = 2; d3 <= max3; d3 += 2) {
        // TODO: Check if d2 is 2, 3, 5 or 7 and
        // print the 3 digits one after another
      }
}
```
[/code-editor]
[task-description]
Write a function to **generate PIN codes** following certain rules. It: 
* Receives **3 digits**: **max1**, **max2**, **max3** (each is an upper limit)
* Generates unique 3-digit **PIN codes**, matching the following:
    * Each digit is **within its range**: \[1..max1\], \[1..max2\], \[1..max3\]
    * The **first** and the **third digit** must be **even**
    * The **second digit** must be a **prime number** in the range \[2…7\]
* Prints the PIN codes in increasing order
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|222|
|5|224|
|5|232|
||234|
||252|
||254|
[/slide]

[slide]
# Problem: Letters Combinations
[code-task title="Letters Combinations" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function lettersCombinations(start, end, x) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a function to generate **3-letter combinations** under certain conditions.It: 
* Receives a start letter **s**, end letter **e** and excluded letter **x**
* Prints all **combinations of 3 letters** in the range \[s…e\], excluding **x**, and their **count**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|a|aaa aac aca acc caa cac cca ccc 8|
|c||
|b||
[/slide]

[slide]
# Solution: Letters Combinations
[code-task title="Letters Combinations" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function lettersCombinations(start, end, x) {
  let counter = 0;
  let startAscii = start.charCodeAt(0);
  let endAscii = end.charCodeAt(0);
  for (let l1 = startAscii; l1 <= endAscii; l1++)
    for (let l2 = startAscii; l2 <= endAscii; l2++)
      for (let l3 = startAscii; l3 <= endAscii; l3++)
        if (l1 !== x && l2 !== x && l3 !== x) {
          // TODO: Convert to char and print the combination
          // TODO: counter++;
        }
  // TODO: Print the counter
}
```
[/code-editor]
[task-description]
Write a function to generate **3-letter combinations** under certain conditions.It: 
* Receives a start letter **s**, end letter **e** and excluded letter **x**
* Prints all **combinations of 3 letters** in the range \[s…e\], excluding **x**, and their **count**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|a|aaa aac aca acc caa cac cca ccc 8|
|c||
|b||
[/slide]

[slide]
# Problem: Happy Numbers
[code-task title="Happy Numbers" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function happyNumbers(n) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a function to generate all 4-digit happy numbers \{d1\}\{d2\}\{d3\}\{d4\} for given a integer **n**
* A number is happy if **d1** + **d2** == **d3** + **d4** == **n**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|1203 1212 1221 1230 2103 2112 2121 2130 3003 3012 3021 3030|
|4|1304 1313 1322 1331 1340 2204 2213 2222 2231 2240 3104 3113 3122 3131 3140 4004 4013 4022 4031 4040|
[/slide]

[slide]
# Problem: Happy Numbers
[code-task title="Happy Numbers" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function happyNumbers(n) {
  let result = '';
  for (let d1 = 1; d1 <= 9; d1++)
    for (let d2 = 0; d2 <= 9; d2++)
      if (d1 + d2 === n)
        for (let d3 = 0; d3 <= 9; d3++)
          for (let d4 = 0; d4 <= 9; d4++)
            if (d3 + d4 === n)
              result += `${d1}${d2}${d3}${d4} `;
  console.log(result);
}
```
[/code-editor]
[task-description]
Write a function to generate all 4-digit happy numbers \{d1\}\{d2\}\{d3\}\{d4\} for given a integer **n**
* A number is happy if **d1** + **d2** == **d3** + **d4** == **n**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|1203 1212 1221 1230 2103 2112 2121 2130 3003 3012 3021 3030|
|4|1304 1313 1322 1331 1340 2204 2213 2222 2231 2240 3104 3113 3122 3131 3140 4004 4013 4022 4031 4040|
[/slide]