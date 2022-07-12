# Challenge 443 - Flash Cards

Create a function that outputs the results of a flashcard. A flashcard is a list of three elements: a number, an operator symbol, and another number. Return the mathematical result of that expression.

There are 4 operators: `+` (addition), `-` (subtraction), `x` (multiplication), and `/` (division). If the flashcard displays a number being divided by zero, e.g. `[3, "/", 0]`, then return `None`/`null`. For division, round to the hundredths place. So `[10, "/", 3]` should return `3.33`.

## Examples
```js
flash(3, "x", 7) ➞ 21

flash(5, "+", 7) ➞ 12

flash(10, "-", 9) ➞ 1

flash(10, "/", 0) ➞ Null

flash(10, "/", 3) ➞ 3.33
```
## Notes

- Flash cards contain only zero or positive numbers.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 
```json
[
    {"args": [3, "x", 7], "return": 21},
    {"args": [5, "+", 7], "return": 12},
    {"args": [10, "-", 9], "return": 1},
    {"args": [10, "/", 0], "return": null},
    {"args": [10, "/", 3], "return": 3.33},
    {"args": [2, "x", 0], "return": 0},
    {"args": [0, "/", 5], "return": 0},
    {"args": [0, "+", 0], "return": 0},
    {"args": [0, "-", 0], "return": 0},
    {"args": [8, "-", 0], "return": 8},
    {"args": [0, "/", 0], "return": null},
    {"args": [3, "/", 8], "return": 0.38}
]
```
## Credits

Found on Edabit: [Flash Cards](https://edabit.com/challenge/ZZsnGAjYLyosG9zmH)
