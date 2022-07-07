# Challenge 492 - One Odd & One Even

Given a two digit number, return `True` if that number contains one even and one odd digit.

## Examples
```python
one_odd_one_even(12) ➞ True

one_odd_one_even(55) ➞ False

one_odd_one_even(22) ➞ False
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def one_odd_one_even(number: int) -> bool:
    return False  # Put your code here!!!


test(492, one_odd_one_even)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            10
        ],
        "return": true
    },
    {
        "args": [
            11
        ],
        "return": false
    },
    {
        "args": [
            12
        ],
        "return": true
    },
    {
        "args": [
            13
        ],
        "return": false
    },
    {
        "args": [
            14
        ],
        "return": true
    },
    {
        "args": [
            15
        ],
        "return": false
    },
    {
        "args": [
            16
        ],
        "return": true
    },
    {
        "args": [
            17
        ],
        "return": false
    },
    {
        "args": [
            18
        ],
        "return": true
    },
    {
        "args": [
            19
        ],
        "return": false
    },
    {
        "args": [
            20
        ],
        "return": false
    },
    {
        "args": [
            30
        ],
        "return": true
    },
    {
        "args": [
            31
        ],
        "return": false
    },
    {
        "args": [
            40
        ],
        "return": false
    },
    {
        "args": [
            41
        ],
        "return": true
    }
]
```
## Credits

Found on Edabit: One Odd and One Even(https://edabit.com/challenge/GPodAAMFqz9sLWmAy)
