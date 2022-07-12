# Challenge 495 - Number Split

Given a number, return a list containing the two halves of the number. If the number is odd, make the rightmost number higher.

## Examples
```python
number_split(4) ➞ [2, 2]

number_split(10) ➞ [5, 5]

number_split(11) ➞ [5, 6]

number_split(-9) ➞ [-5, -4]
```
## Notes

- All numbers will be integers.
- You can expect negative numbers too.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def number_split(number: int) -> list[int]:
    return []  # Put your code here!!!


test(495, number_split)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            4
        ],
        "return": [
            2,
            2
        ]
    },
    {
        "args": [
            10
        ],
        "return": [
            5,
            5
        ]
    },
    {
        "args": [
            11
        ],
        "return": [
            5,
            6
        ]
    },
    {
        "args": [
            0
        ],
        "return": [
            0,
            0
        ]
    },
    {
        "args": [
            1
        ],
        "return": [
            0,
            1
        ]
    },
    {
        "args": [
            -4
        ],
        "return": [
            -2,
            -2
        ]
    },
    {
        "args": [
            -5
        ],
        "return": [
            -3,
            -2
        ]
    },
    {
        "args": [
            -9
        ],
        "return": [
            -5,
            -4
        ]
    }
]
```
## Credits

Found on Edabit: [Number Split](https://edabit.com/challenge/9f3Mi6vHNcm8vRcSh)
