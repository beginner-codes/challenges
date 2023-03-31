# Challenge 634 - Three Lists!

Given three lists of integers, return the sum of integers which are common in all three lists.

## Examples
```python
sum_common([1, 2, 3], [5, 3, 2], [7, 3, 2]) ➞ 5
// 2 & 3 are common in all 3 lists.

sum_common([1, 2, 2, 3], [5, 3, 2, 2], [7, 3, 2, 2]) ➞ 7
// 2, 2 & 3 are common in all 3 lists.

sum_common([1], [1], [2]) ➞ 0
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def sum_common(list_a: list[int], list_b: list[int], list_c: list[int]) -> int:
    return 0  # Put your code here!!!


test(634, sum_common)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                1,
                2,
                2,
                3
            ],
            [
                5,
                3,
                2,
                2
            ],
            [
                7,
                3,
                2,
                2
            ]
        ],
        "return": 7
    },
    {
        "args": [
            [
                1
            ],
            [
                1
            ],
            [
                1
            ]
        ],
        "return": 1
    },
    {
        "args": [
            [
                1
            ],
            [
                1
            ],
            [
                2
            ]
        ],
        "return": 0
    },
    {
        "args": [
            [
                1,
                2,
                2,
                3,
                2
            ],
            [
                5,
                3,
                2,
                2,
                1
            ],
            [
                7,
                3,
                2,
                2,
                1
            ]
        ],
        "return": 8
    },
    {
        "args": [
            [
                1,
                2,
                3
            ],
            [
                5,
                3,
                2
            ],
            [
                7,
                3,
                2
            ]
        ],
        "return": 5
    }
]
```
## Credits

Found on Edabit: [Three Lists!](https://edabit.com/challenge/GQjKJtG6dqeyBSCqX)
