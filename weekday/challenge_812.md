# Challenge 812 - Check If Lines Are Parallel

Given two lines, determine whether they are parallel.

Lines are represented by a list `[a, b, c]`, which corresponds to the line `ax+by=c`.

## Examples
```python
lines_are_parallel([1, 2, 3], [1, 2, 4]) ➞ True
# x+2y=3 and x+2y=4 are parallel.

lines_are_parallel([2, 4, 1], [4, 2, 1]) ➞ False
# 2x+4y=1 and 4x+2y=1 are not parallel.

lines_are_parallel([0, 1, 5], [0, 1, 5]) ➞ True
# Lines are parallel to themselves.
```
## Notes

- Two lines are parallels if they have the same slope. If the slopes are different, the lines are not parallel.
- All coefficients will be integers (whole numbers).

## Hint

The first letter of the term should always be capital, even if it's "b".

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


def lines_are_parallel(line_a: list[int], line_b: list[int]) -> bool:
    return False  # Put your code here!!!


test(812, lines_are_parallel)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                2,
                5,
                0
            ],
            [
                20,
                50,
                10
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                0,
                1,
                5
            ],
            [
                0,
                1,
                5
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                1,
                2,
                3
            ],
            [
                1,
                2,
                4
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                400000,
                1,
                0
            ],
            [
                800000,
                2,
                100000
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                -5,
                7,
                100000
            ],
            [
                5,
                -7,
                -200000
            ]
        ],
        "return": true
    }
]
```

## Credits

Found on Edabit: [Check If Lines Are Parallel](https://edabit.com/challenge/8rEEHcmq8rRaTksd7)
