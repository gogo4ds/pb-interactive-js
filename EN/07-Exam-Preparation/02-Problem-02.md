[slide]
# Problem 02
## Description
During the lunch break you want to watch an episode from your favorite series. 

Your task is to write a program that will help you determine whether you have enough time to watch the episode. 

In the lunch break you spend time to have lunch and to unwind. 

The time for lunch will be 1/8 of the break time and the time for relaxing will be 1/4 of the break time.

## Input
You receive 3 lines from the console:
- Name of the series - string
- Duration of an episode - whole number in the range [10… 90]
- Duration of the break - whole number in the range [10… 120]

## Output
Print on the console one line:
- If the time is enough to watch the episode: "You have enough time to watch \{name of the series\} and left with \{time left\} minutes free time."
- If the time is not enough: "You don't have enough time to watch \{name of the series\}, you need \{time needed\} more minutes."
Round the time up to the nearest whole number.

[code-task title="Problem-02" executionStrategy="javascript-code" requiresInput]
[code-editor language=javascript]
```
function solve(input) {
	// Write your code here
}
```
[/code-editor]
[task-description]
## Input
Name of the series - Game of Thrones

Duration of an episode - 60

Duration of the break - 96

## Output
You have enough time to watch Game of Thrones and left with 0 minutes free time.

## Comments
Time for lunch: 96 * 1/8 = 12.0

Time to unwind: 96 * 1/4 = 24.0

Time left: 96 - 12 - 24 = 60

The time we have left is bigger or equal to the duration of the episode, so we print the suitable output. 
[/task-description]
[code-io /]
[/code-task]
[/slide]