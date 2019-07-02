[slide]
# Problem 05
## Description
You are hired by a TV company to write a program that calculate whether it is possible for customers to purchase the desired series. You have a budget and number of series that the user will want to purchase. Each series has a title and price.
Some of the series have a discount:
- Thrones – 50%
- Lucifer – 40%	
- Protector – 30%
- TotalDrama – 20%
- Area – 10%

## Input
You receive from the console:
- Budget - real number in the range [10.0… 100.0]
- Count series - n – whole number in the range [1… 10]

For each series you receive two lines:
- Name of the series - string
- Price for a series - real number in the range [1.0… 15.0]

## Output
Print one line on the console:
- If your budget is greater than or equal to the price of the series: "You bought all the series and left with \{money left\}$"
- If your budget is less than the price of the series: "You need \{money needed\}$ more to buy the series!"

The result must be formatted to two digits after the decimal point.
[code-task title="Problem-05" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function solve(input) {
	// Write your code here
}
```
[/code-editor]
[task-description]
## Input
Budget - 10

Count series - 3

Name of the first series - Thrones

Price for the first series - 5

Name of the second series - Riverdale

Price for the second series - 5

Name of the third series - Gotham

Price for the third series - 2

## Output
You bought all the series and left with 0.50$

## Comments
You receive budget – 10$ and count of series - 3. The first series is Thrones with price 5$, which has 50% discount from the price 5 - 50% = 2.50$. The second series is Riverdale, which does not have a discount on the price. The third series also does not have a discount. Price of series is 2.50 + 5 + 2 = 9.50$. Your budget is bigger than the price of series, so you can buy them.
[/task-description]
[code-io /]
[/code-task]
[/slide]