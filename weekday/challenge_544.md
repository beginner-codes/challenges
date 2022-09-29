# Challenge 544 - Magic Date

Determine whether a date is a magic date. Here are the rules for a magic date:

- `mm * dd` is a 1-digit number that matches the last digit of `yyyy`
- `mm * dd` is a 2-digit number that matches the last 2 digits of `yyyy`
- `mm * dd` is a 3-digit number that matches the last 3 digits of `yyyy`

The function should return `True` if the date is magic, or `False` if it is not.

## Examples
```python
magic("1 1 2011") ➞ True

magic("4 1 2001") ➞ False

magic("5 2 2010") ➞ True

magic("9 2 2011") ➞ False
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def magic(date: str) -> bool:
    return False # Put your code here!!!


test(544, magic)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "3 3 2009"
        ],
        "return": true
    },
    {
        "args": [
            "2 4 2008"
        ],
        "return": true
    },
    {
        "args": [
            "9 2 2011"
        ],
        "return": false
    },
    {
        "args": [
            "4 1 2001"
        ],
        "return": false
    },
    {
        "args": [
            "1 1 2011"
        ],
        "return": true
    }
]
```
## Credits

Found on Edabit: [Magic Date](https://edabit.com/challenge/GoGbZtXDYPDCfeBz8)
