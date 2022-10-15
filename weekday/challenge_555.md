# Challenge 555 - Mowing the Lawn

Create a function that takes in an array of grass heights and a variable sequence of lawn mower cuts and outputs the array of successive grass heights.

If after a cut, any single element in the array reaches zero or negative, return "Done" instead of the array of new heights.

A demo:
```python
cutting_grass([3, 4, 4, 4], 1, 1, 1) ➞ [[2, 3, 3, 3], [1, 2, 2, 2], "Done"]

# 1st cut shaves off 1: [3, 4, 4, 4] ➞ [2, 3, 3, 3]
# 2nd cut shaves off 1: [2, 3, 3, 3] ➞ [1, 2, 2, 2]
# 3rd cut shaves off 1: [1, 2, 2, 2]➞ [0, 1, 1, 1], but one element reached zero so we return "Done".
```
## Examples
```python
cutting_grass([4, 4, 4, 4], 1, 1, 1, 1)
➞ [[3, 3, 3, 3], [2, 2, 2, 2], [1, 1, 1, 1], "Done"]

cutting_grass([5, 6, 7, 5], 1, 2, 1)
➞ [[4, 5, 6, 4], [2, 3, 4, 2], [1, 2, 3, 1]]

cutting_grass([8, 9, 9, 8, 8], 2, 3, 2, 1)
➞ [[6, 7, 7, 6, 6], [3, 4, 4, 3, 3], [1, 2, 2, 1, 1], "Done"]

cutting_grass([1, 0, 1, 1], 1, 1, 1) ➞ ["Done", "Done", "Done"]
```
## Notes

- The number of lawn cuts is variable.
- There will be at least one cut.
- Return `"Done"` onwards for each additional cut if the grass has already been completely mowed.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test
from typing import Literal


def cutting_grass(grass: list[int], *cuts: int) -> list[list[int] | Literal["Done"]]:
    return [] # Put your code here!!!


test(555, cutting_grass)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                4,
                2,
                2
            ],
            2,
            1,
            1
        ],
        "return": [
            "Done",
            "Done",
            "Done"
        ]
    },
    {
        "args": [
            [
                4,
                4,
                4,
                4
            ],
            1,
            1,
            1,
            1
        ],
        "return": [
            [
                3,
                3,
                3,
                3
            ],
            [
                2,
                2,
                2,
                2
            ],
            [
                1,
                1,
                1,
                1
            ],
            "Done"
        ]
    },
    {
        "args": [
            [
                1,
                0,
                1,
                1
            ],
            1,
            1,
            1
        ],
        "return": [
            "Done",
            "Done",
            "Done"
        ]
    },
    {
        "args": [
            [
                5,
                6,
                7,
                5
            ],
            1,
            2,
            1
        ],
        "return": [
            [
                4,
                5,
                6,
                4
            ],
            [
                2,
                3,
                4,
                2
            ],
            [
                1,
                2,
                3,
                1
            ]
        ]
    },
    {
        "args": [
            [
                8,
                9,
                9,
                8,
                8
            ],
            2,
            3,
            2,
            1
        ],
        "return": [
            [
                6,
                7,
                7,
                6,
                6
            ],
            [
                3,
                4,
                4,
                3,
                3
            ],
            [
                1,
                2,
                2,
                1,
                1
            ],
            "Done"
        ]
    }
]
```
## Credits

Found on Edabit: [Mowing the Lawn](https://edabit.com/challenge/4jNjHdZ2hmMh23pRg)
