# Challenge 828 - Matrix Multiplication

Create a function that multiplies two matrices (2x2 each).

## Examples
```python
matrix_mult([[4, 2],[3, 1]], [[5, 6], [3, 8]]) ➞ [[26, 40], [18, 26]]

matrix_mult([[3, 6],[4, 5]], [[8, 1], [7, 2]]) ➞ [[66, 15], [67, 14]]

matrix_mult([[7, 5],[2, 2]], [[6, 7], [3, 2]]) ➞ [[57, 59], [18, 18]]
```
## Notes

- Limit yourself to 2x2 matrices

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
from typing import TypeAlias
from beginnercodes.challenges import test


Row: TypeAlias = list[int]
Matrix: TypeAlias = list[Row]


def matrix_mult(matrix_a: Matrix, matrix_b: Matrix) -> Matrix:
    return []  # Put your code here!!!


test(828, matrix_mult)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                [
                    7,
                    5
                ],
                [
                    2,
                    2
                ]
            ],
            [
                [
                    6,
                    7
                ],
                [
                    3,
                    2
                ]
            ]
        ],
        "return": [
            [
                57,
                59
            ],
            [
                18,
                18
            ]
        ]
    },
    {
        "args": [
            [
                [
                    3,
                    6
                ],
                [
                    4,
                    5
                ]
            ],
            [
                [
                    8,
                    1
                ],
                [
                    7,
                    2
                ]
            ]
        ],
        "return": [
            [
                66,
                15
            ],
            [
                67,
                14
            ]
        ]
    },
    {
        "args": [
            [
                [
                    4,
                    2
                ],
                [
                    3,
                    1
                ]
            ],
            [
                [
                    5,
                    6
                ],
                [
                    3,
                    8
                ]
            ]
        ],
        "return": [
            [
                26,
                40
            ],
            [
                18,
                26
            ]
        ]
    }
]
```

## Credits

Found on Edabit: [Matrix Multiplication](https://edabit.com/challenge/dfep4NR2twAFTdt9k)
