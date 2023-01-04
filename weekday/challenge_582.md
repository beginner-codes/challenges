# Challenge 582 - Friday the 13th

Given the month and year as numbers, return whether that month contains a Friday 13th.

## Examples
```python
has_friday_13(3, 2020) ➞ True

has_friday_13(10, 2017) ➞ True

has_friday_13(1, 1985) ➞ False
```
## Notes

- January will be given as `1`, February as `2`, etc.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def has_friday_13(month: int, year: int) -> bool:
    return False  # Put your code here!!!


test(582, has_friday_13)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            3,
            2043
        ],
        "return": true
    },
    {
        "args": [
            2,
            1759
        ],
        "return": false
    },
    {
        "args": [
            11,
            2015
        ],
        "return": true
    },
    {
        "args": [
            8,
            1612
        ],
        "return": false
    },
    {
        "args": [
            3,
            2020
        ],
        "return": true
    }
]
```
## Credits

Found on Edabit: [Friday the 13th](https://edabit.com/challenge/Xkc2iAjwCap2z9N5D)
