# Challenge 511 - Even All the Way

Given a list of numbers, return a list which contains all the even numbers in the original list, which also have even indices.

## Examples
```python
get_only_evens([1, 3, 2, 6, 4, 8]) ➞ [2, 4]

get_only_evens([0, 1, 2, 3, 4]) ➞ [0, 2, 4]

get_only_evens([1, 2, 3, 4, 5]) ➞ []
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def get_only_evens(numbers: list[int]) -> list[int]:
    return []  # Put your code here!!!


test(511, get_only_evens)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                1,
                3,
                2,
                6,
                4,
                8
            ]
        ],
        "return": [
            2,
            4
        ]
    },
    {
        "args": [
            [
                0,
                1,
                2,
                3,
                4
            ]
        ],
        "return": [
            0,
            2,
            4
        ]
    },
    {
        "args": [
            [
                1,
                2,
                3,
                4,
                5
            ]
        ],
        "return": []
    },
    {
        "args": [
            [
                37,
                26,
                18,
                42,
                2,
                30
            ]
        ],
        "return": [
            18,
            2
        ]
    },
    {
        "args": [
            [
                49,
                41,
                30,
                44,
                26,
                0,
                5
            ]
        ],
        "return": [
            30,
            26
        ]
    },
    {
        "args": [
            [
                47,
                47,
                12,
                3,
                48
            ]
        ],
        "return": [
            12,
            48
        ]
    },
    {
        "args": [
            [
                30,
                26,
                0,
                13,
                20,
                38,
                50,
                2
            ]
        ],
        "return": [
            30,
            0,
            20,
            50
        ]
    },
    {
        "args": [
            [
                34,
                21,
                38,
                28,
                13,
                8,
                26,
                29,
                24,
                5
            ]
        ],
        "return": [
            34,
            38,
            26,
            24
        ]
    },
    {
        "args": [
            [
                47,
                31,
                24,
                37,
                29,
                41,
                31,
                49,
                4,
                24
            ]
        ],
        "return": [
            24,
            4
        ]
    }
]
```
## Credits

Found on Edabit: [Even All the Way](https://edabit.com/challenge/TJxPyuusqjtWF9rff)
