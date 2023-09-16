# Challenge 752 - Maximum Product of Digits

Write a function that returns all numbers less than or equal to N that have the highest possible product of their digits.

## Examples
```python
max_product(8) ➞ [8]
# 8 is the largest possible product of digits under 8

max_product(27) ➞ [27]
# 27 is the largest product of digits (2 * 7 = 14) under 27

max_product(211) ➞ [99, 199]
# 99 and 199 are both the largest product of digits (9 * 9 = 81, 1 * 9 * 9 = 81) under 211 

max_product(9578) ➞ [8999]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. *
*[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a
key `args` that are a list of parameters your function should take. The `return` key is what your function should return
given the `args`.

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your
solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:

```python
from __future__ import annotations
from beginnercodes.challenges import test


def max_product(number: int) -> list[int]:
    return []  # Put your code here!!!


test(752, max_product)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            917
        ],
        "return": [
            899
        ]
    },
    {
        "args": [
            11111
        ],
        "return": [
            9999
        ]
    },
    {
        "args": [
            26
        ],
        "return": [
            26
        ]
    },
    {
        "args": [
            41111
        ],
        "return": [
            39999
        ]
    },
    {
        "args": [
            211
        ],
        "return": [
            99,
            199
        ]
    }
]
```

## Credits

Found on Edabit: [Maximum Product of Digits](https://edabit.com/challenge/oRwcjPMkyznd2ybRW)
