# Challenge 625 - Dice Score

Greed is a dice game played with five six-sided dice. Your mission is to score a throw according to these rules:
```
 Three 1's => 1000 points
 Three 6's =>  600 points
 Three 5's =>  500 points
 Three 4's =>  400 points
 Three 3's =>  300 points
 Three 2's =>  200 points
 One   1   =>  100 points
 One   5   =>   50 point
```
See the below examples for a better understanding:
```
 Throw       Score
 ---------   ------------------
 5 1 3 4 1   250:  50 (for the 5) + 2 * 100 (for the 1s)
 1 1 1 3 1   1100: 1000 (for three 1s) + 100 (for the other 1)
 2 4 4 5 4   450:  400 (for three 4s) + 50 (for the 5)
```
Create a function that takes a list of five six-sided throw values and returns the final calculated dice score.

## Examples
```python
dice_score([2, 3, 4, 6, 2]) ➞ 0

dice_score([4, 4, 4, 3, 3]) ➞ 400

dice_score([2, 4, 4, 5, 4]) ➞ 450
```
## Notes

- A single die can only be counted once in each roll. For example, a given "5" can only be counted as a part of the triplet (contributing to the 500 points) or as a single 50 points, but not both in the same roll.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def sort_authors(authors: list[str]) -> list[str]:
    return []  # Put your code here!!!


test(624, sort_authors)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                4,
                4,
                4,
                3,
                3
            ]
        ],
        "return": 400
    },
    {
        "args": [
            [
                5,
                5,
                5,
                3,
                3
            ]
        ],
        "return": 500
    },
    {
        "args": [
            [
                6,
                6,
                6,
                3,
                3
            ]
        ],
        "return": 600
    },
    {
        "args": [
            [
                3,
                4,
                5,
                3,
                3
            ]
        ],
        "return": 350
    },
    {
        "args": [
            [
                2,
                4,
                4,
                5,
                4
            ]
        ],
        "return": 450
    }
]
```
## Credits

Found on Edabit: [Dice Score](https://edabit.com/challenge/6FaERG8x8Y6MYmoYF)
