# Challenge 587 - Digits Sum Root

Create a function that takes a number and returns one digit that is the result of summing all the digits of the input number. When the sum of the digits consists of more than one digit, repeat summing until you get one digit.

## Examples
```python
root_digit(123) ➞ 6
# 1 + 2 + 3 = 6

root_digit(999888777) ➞ 9

root_digit(1238763636555555555555) ➞ 6
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def root_digit(number: int) -> int:
    return 0  # Put your code here!!!


test(587, root_digit)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            0
        ],
        "return": 0
    },
    {
        "args": [
            1238222222222222222263612387636361238763636
        ],
        "return": 7
    },
    {
        "args": [
            999888777
        ],
        "return": 9
    },
    {
        "args": [
            1111177999888777999888777999888777
        ],
        "return": 1
    },
    {
        "args": [
            1238763636555555555555
        ],
        "return": 6
    }
]
```
## Credits

Found on Edabit: [Digits Sum Root](https://edabit.com/challenge/veCWQHJNgeZQCNbdY)
