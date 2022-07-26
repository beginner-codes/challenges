# Challenge 505 - Harshad Numbers

A Harshad (also called Niven) number is any number divisible by the sum of its digits. For example, `666` is divisible by `6 + 6 + 6`, so it is a Harshad number.

Write a function to determine whether a number is a Harshad number.

## Examples
```python
is_harshad(209) ➞ True

is_harshad(41) ➞ False

is_harshad(12255) ➞ True
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def is_harshad(number: int) -> bool:
    return False  # Put your code here!!!


test(505, is_harshad)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            0
        ],
        "return": false
    },
    {
        "args": [
            15
        ],
        "return": false
    },
    {
        "args": [
            990
        ],
        "return": true
    },
    {
        "args": [
            461
        ],
        "return": false
    },
    {
        "args": [
            297
        ],
        "return": false
    },
    {
        "args": [
            345
        ],
        "return": false
    },
    {
        "args": [
            529
        ],
        "return": false
    },
    {
        "args": [
            839
        ],
        "return": false
    },
    {
        "args": [
            281
        ],
        "return": false
    },
    {
        "args": [
            252
        ],
        "return": true
    }
]
```
## Credits

Found on Edabit: [Harshad Numbers](https://edabit.com/challenge/ZDDyfBFBWMotQSYin)
