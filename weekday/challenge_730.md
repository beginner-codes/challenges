# Challenge 730 - Minimum Difference Pair

Given a list of numbers, return the pair of numbers that give the minimum absolute difference. Return the pair as a list, sorted in ascending order. If multiple pairs have the same difference, return the pair with the smallest sum.

## Examples
```python
min_difference_pair([40, 16, 8, 17, 15]) ➞ [15, 16]
# [15, 16] has smaller sum than [16, 17]

min_difference_pair([1, -31, -27, -18, -48, -15, -11, -34]) ➞ [-34, -31]

min_difference_pair([0, 2, 35, 42, 45, 14, -6, -1]) ➞ [-1, 0]

min_difference_pair([32, 33, 4, 6, 48, 18, 20, -7, -4, 31]) ➞ [31, 32]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def min_difference_pair(numbers: list[int]) -> list[int]:
    return []  # Put your code here!!!


test(730, min_difference_pair)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                15,
                2,
                17,
                19,
                5,
                -4
            ]
        ],
        "return": [
            15,
            17
        ]
    },
    {
        "args": [
            [
                27,
                49,
                28,
                13,
                -9,
                -2,
                50
            ]
        ],
        "return": [
            27,
            28
        ]
    },
    {
        "args": [
            [
                22,
                -3,
                4,
                1,
                46,
                21,
                0,
                29
            ]
        ],
        "return": [
            0,
            1
        ]
    },
    {
        "args": [
            [
                13,
                7,
                39,
                30,
                17,
                6,
                38,
                14
            ]
        ],
        "return": [
            6,
            7
        ]
    },
    {
        "args": [
            [
                18,
                -3,
                -10,
                4,
                19,
                -6,
                15,
                20,
                14,
                6
            ]
        ],
        "return": [
            14,
            15
        ]
    }
]
```
## Credits

Found on Edabit: [Minimum Difference Pair](https://edabit.com/challenge/oLmAshdKHWLP3ck7e)
