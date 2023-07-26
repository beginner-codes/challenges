# Challenge 713 - Straight Digital Numbers

In this challenge, you have to establish if the digits of a given number form a straight arithmetic sequence (either increasing or decreasing). A straight sequence has an equal step between every pair of digits.

Given an integer, implement a function that returns:

- `-1` if the number is lower than 100 or if its digits are not an arithmetic sequence.
- `0` if the number has a single repeating digit.
- An integer being the absolute value of the step of the sequence if the number's digits are a straight arithmetic sequence.

## Examples
```python
straight_digital(123) ➞ 1
# 2 - 1 = 1 | 3 - 2 = 1

straight_digital(753) ➞ 2
# 5 - 7 = -2 | 3 - 5 = -2

straight_digital(666) ➞ 0

straight_digital(124) ➞ -1
# 2 - 1 = 1 | 4 - 2 = 2
# A valid sequence has always the same step between its digits.

straight_digital(99) ➞ -1
# The number is lower than 100.
```
## Notes

- The step of the sequence can be either positive or negative. 

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def straight_digital(number: int) -> int:
    return 0  # Put your code here!!!


test(713, straight_digital)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            -123456789
        ],
        "return": -1
    },
    {
        "args": [
            13579
        ],
        "return": 2
    },
    {
        "args": [
            124
        ],
        "return": -1
    },
    {
        "args": [
            147
        ],
        "return": 3
    },
    {
        "args": [
            666
        ],
        "return": 0
    }
]
```
## Credits

Found on Edabit: [Straight Digital Numbers](https://edabit.com/challenge/nmoohLwP962r6P355)
