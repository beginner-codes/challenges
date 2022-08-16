# Challenge 519 - Preventing the Collapse of the Universe

Dividing by `0` is a huge mistake and should be avoided at all costs.

Create a function that when given a math expression as a string returns `True` if at any point the expression involves dividing by `0`.

## Examples
```python
catch_zero_division("2 / 0") ➞ True

catch_zero_division("4 / (2 + 3 - 5)") ➞ True

catch_zero_division("2 * 5 - 10") ➞ False
```
## Notes

- Multiplication signs will be given as an asterisk `*`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def catch_zero_division(expression: str) -> bool:
    return False # Put your code here!!!


test(519, catch_zero_division)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "0+0+0+0+0+0+0"
        ],
        "return": false
    },
    {
        "args": [
            "0 + 0 + (3 / (3 - 3))"
        ],
        "return": true
    },
    {
        "args": [
            "3 / 0"
        ],
        "return": true
    },
    {
        "args": [
            "4 / (2 + 3 - 5)"
        ],
        "return": true
    },
    {
        "args": [
            "0 / 0"
        ],
        "return": true
    },
    {
        "args": [
            "3 / 0"
        ],
        "return": true
    },
    {
        "args": [
            "23 - 23 / 23"
        ],
        "return": false
    },
    {
        "args": [
            "2 * 5 - 3"
        ],
        "return": false
    },
    {
        "args": [
            "2 / 0"
        ],
        "return": true
    },
    {
        "args": [
            "5343456787543234567 / 743044830483009043909003"
        ],
        "return": false
    }
]
```
## Credits

Found on Edabit: [Preventing the Collapse of the Universe](https://edabit.com/challenge/5raq8tMwYrXq2ncwf)
