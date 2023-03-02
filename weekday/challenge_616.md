# Challenge 616 - Shared Digits

Create a function that returns `True` if each pair of adjacent numbers in a list shares at least one digit and `False` otherwise.

## Examples
```python
shared_digits([33, 53, 6351, 12, 2242, 44]) ➞ True
# 33 and 53 share 3, 53 and 6351 share 3 and 5, etc.

shared_digits([1, 11, 12, 13, 14, 15, 16]) ➞ True

shared_digits([33, 44, 55, 66, 77]) ➞ False

shared_digits([1, 12, 123, 1234, 1235, 6789]) ➞ False
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def shared_digits(numbers: list[int]) -> bool:
    return False  # Put your code here!!!


test(616, shared_digits)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                5,
                55,
                665,
                4444,
                65,
                66,
                76,
                78,
                989
            ]
        ],
        "return": false
    },
    {
        "args": [
            [
                5,
                65,
                66,
                76,
                78
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                33,
                53,
                6351,
                12,
                2242,
                44
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                1,
                12,
                123,
                1234,
                1235,
                6789
            ]
        ],
        "return": false
    },
    {
        "args": [
            [
                5789,
                798,
                98,
                995,
                599,
                699
            ]
        ],
        "return": true
    }
]
```
## Credits

Found on Edabit: [Shared Digits](https://edabit.com/challenge/rk4nyFSXc6vcSWMWH)
