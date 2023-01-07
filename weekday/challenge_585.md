# Challenge 585 - Sort the String

Create a function that takes a string consisting of lowercase letters, uppercase letters and numbers and returns the string sorted in the same way as the examples below.

Examples
```js
sorting("eA2a1E") ➞ "aAeE12"
// Don't repeat letters.

sorting("Re4r") ➞ "erR4"

sorting("6jnM31Q") ➞ "jMnQ136"

sorting("846ZIbo") ➞ "bIoZ468"
```
## Notes

- Don't repeat letters (numbers can be repeated).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def sorting(string: str) -> str:
    return ""  # Put your code here!!!


test(585, sorting)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "eA2a1E"
        ],
        "return": "aAeE12"
    },
    {
        "args": [
            "846ZIbo"
        ],
        "return": "bIoZ468"
    },
    {
        "args": [
            "2lZduOg1jB8SPXf5rakC37wIE094Qvm6Tnyh"
        ],
        "return": "aBCdEfghIjklmnOPQrSTuvwXyZ0123456789"
    },
    {
        "args": [
            "6jnM31Q"
        ],
        "return": "jMnQ136"
    },
    {
        "args": [
            "f5Eex"
        ],
        "return": "eEfx5"
    },
    {
        "args": [
            "Re4r"
        ],
        "return": "erR4"
    }
]
```
## Credits

Found on Edabit: [Sort the String](https://edabit.com/challenge/fRZMqCpyxpSgmriQ6)
