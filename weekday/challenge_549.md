# Challenge 549 - Does a Number Exist?

Create a function which validates whether a string is a number.

## Examples
```python
valid_str_number("3.2") ➞ True

valid_str_number("324") ➞ True

valid_str_number("54..4") ➞ False

valid_str_number("number") ➞ False
```
## Notes

- Accept numbers such as .5 and 0003.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def valid_str_number(string: str) -> bool:
    return False # Put your code here!!!


test(549, valid_str_number)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "54..4"
        ],
        "return": false
    },
    {
        "args": [
            "3.2"
        ],
        "return": true
    },
    {
        "args": [
            "000.000"
        ],
        "return": true
    },
    {
        "args": [
            "number"
        ],
        "return": false
    },
    {
        "args": [
            "0000000"
        ],
        "return": true
    },
    {
        "args": [
            "1234321"
        ],
        "return": true
    },
    {
        "args": [
            "3.e"
        ],
        "return": false
    },
    {
        "args": [
            "324"
        ],
        "return": true
    },
    {
        "args": [
            ".5"
        ],
        "return": true
    },
    {
        "args": [
            ".42.3"
        ],
        "return": false
    },
    {
        "args": [
            "03"
        ],
        "return": true
    }
]
```
## Credits

Found on Edabit: [Does a Number Exist?](https://edabit.com/challenge/sCH5gcyoRqq3Gfzyi)
