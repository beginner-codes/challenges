# Challenge 543 - Flatten the Curve

Given a list of integers, replace every number with the mean of all numbers.

## Examples
```python
flatten_the_curve([1, 2, 3, 4, 5]) ➞ [3, 3, 3, 3, 3]

flatten_the_curve([0, 0, 0, 2, 7, 3]) ➞ [2, 2, 2, 2, 2, 2]

flatten_the_curve([4]) ➞ [4]

flatten_the_curve([]) ➞ []
```
## Notes

- Round averages to 1 decimal point.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def flatten_the_curve(numbers: list[int]) -> list[int]:
    return [] # Put your code here!!!


test(543, flatten_the_curve)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                23,
                -13,
                -13,
                -15,
                13
            ]
        ],
        "return": [
            -1.0,
            -1.0,
            -1.0,
            -1.0,
            -1.0
        ]
    },
    {
        "args": [
            [
                -13,
                0,
                -18
            ]
        ],
        "return": [
            -10.3,
            -10.3,
            -10.3
        ]
    },
    {
        "args": [
            [
                -19,
                29,
                -15,
                30,
                -17
            ]
        ],
        "return": [
            1.6,
            1.6,
            1.6,
            1.6,
            1.6
        ]
    },
    {
        "args": [
            [
                22,
                -12,
                0,
                -19,
                2,
                17,
                -11,
                6
            ]
        ],
        "return": [
            0.6,
            0.6,
            0.6,
            0.6,
            0.6,
            0.6,
            0.6,
            0.6
        ]
    },
    {
        "args": [
            [
                -7,
                13,
                18
            ]
        ],
        "return": [
            8.0,
            8.0,
            8.0
        ]
    }
]
```
## Credits

Found on Edabit: [Flatten the Curve](https://edabit.com/challenge/WsHSAEBQW6F7nsMjr)
