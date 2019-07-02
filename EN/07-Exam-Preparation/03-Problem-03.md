[slide]
# Problem 03
## Description
For the upcoming premiere of three popular productions a local cinema has hired you to write a software that calculates the price, which the clients have to pay, depending on the movie and the offer they have chosen.

|   | John Wick | Star Wars | Jumanji |
|---|---|---|---|
| Drink | 12$ | 18$ | 9$ |
| Popcorn | 15$ | 25$ | 11$ |
| Menu | 19$ | 30$ | 14$ |

Write a program that calculates the price that has to be paid. Keep in mind that there are discounts:
- If the chosen movie is "Star Wars" and at least four tickets are bought, there is 30% family discount.
- If the chosen movie is "Jumanji" and the tickets bought are exactly two, there is 15% discount for two.

## Input
You receive 3 lines from the console:
- First line - movie - string: "John Wick", "Star Wars" or "Jumanji"
- Second line - offer - string:"Drink", "Popcorn" or "Menu"
- Third line - count tickets – whole number in the range [1… 30]

## Output
Print one line on the console: "Your bill is \{total price\}$"
 * The price must be formatted to two digits after the decimal point.

[code-task title="Problem-03" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function solve(input) {
	// Write your code here
}
```
[/code-editor]
[task-description]
## Input
Movie - John Wick

Offer - Drink

Count tickets – 6

## Output
Your bill is 72.00$

## Comments
The movie is Star Wars and popcorn is chosen.

The price for one ticket is 25$

4 tickets each 25$ -> 100$

For this movie there is 30% discount for 4 or more people. 

30% of 100 -> 30 

100 – 30 -> 70$ is the total price
[/task-description]
[code-io /]
[/code-task]
[/slide]