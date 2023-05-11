# Challenge 661 - The Bottom of the Matrix

This challenge concerns square matrices (same number of rows and columns) as the below example illustrates:
```python
[
  [1, 2, 3],
  [4, 5, 6],
  [7, 8, 9]
]
```
The entries in the diagonal line from the top left to the bottom right form the main diagonal of the matrix. In this case, 1,5,9 form the main diagonal.

Write a function that returns the matrix obtained by replacing the entries above the main diagonal with 0s.

For example, for the matrix above you should return:
```python
[
  [1, 0, 0],
  [4, 5, 0],
  [7, 8, 9]
]
```
## Examples
```python
lower_triangle([
  [1, 2, 3],
  [4, 5, 6],
  [7, 8, 9]
]) ➞ [
  [1, 0, 0],
  [4, 5, 0],
  [7, 8, 9]
]

lower_triangle([
  [5, 7],
  [7, 9]
]) ➞ [
  [5, 0],
  [7, 9]
]

lower_triangle([
  [1, 8, 8, 1],
  [2, 7, 7, 2],
  [3, 6, 6, 3],
  [4, 5, 5, 4]
]) ➞ [
  [1, 0, 0, 0],
  [2, 7, 0, 0],
  [3, 6, 6, 0],
  [4, 5, 5, 4]
]
```
## Notes

- As in the examples, the size of the matrices will vary (but they will always be square).
- In Linear Algebra, matrices with 0s above the diagonal are called lower triangular matrices.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def lower_triangle(matrix: list[list[int]]) -> list[list[int]]:
    return []  # Put your code here!!!


test(661, lower_triangle)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                [
                    0,
                    1,
                    2,
                    3,
                    4
                ],
                [
                    1,
                    2,
                    3,
                    4,
                    5
                ],
                [
                    2,
                    3,
                    4,
                    5,
                    6
                ],
                [
                    3,
                    4,
                    5,
                    6,
                    7
                ],
                [
                    4,
                    5,
                    6,
                    7,
                    8
                ]
            ]
        ],
        "return": [
            [
                0,
                0,
                0,
                0,
                0
            ],
            [
                1,
                2,
                0,
                0,
                0
            ],
            [
                2,
                3,
                4,
                0,
                0
            ],
            [
                3,
                4,
                5,
                6,
                0
            ],
            [
                4,
                5,
                6,
                7,
                8
            ]
        ]
    },
    {
        "args": [
            [
                [
                    1,
                    2,
                    3
                ],
                [
                    4,
                    5,
                    6
                ],
                [
                    7,
                    8,
                    9
                ]
            ]
        ],
        "return": [
            [
                1,
                0,
                0
            ],
            [
                4,
                5,
                0
            ],
            [
                7,
                8,
                9
            ]
        ]
    },
    {
        "args": [
            [
                [
                    1,
                    0
                ],
                [
                    7,
                    3
                ]
            ]
        ],
        "return": [
            [
                1,
                0
            ],
            [
                7,
                3
            ]
        ]
    },
    {
        "args": [
            [
                [
                    1,
                    8,
                    8,
                    1
                ],
                [
                    2,
                    7,
                    7,
                    2
                ],
                [
                    3,
                    6,
                    6,
                    3
                ],
                [
                    4,
                    5,
                    5,
                    4
                ]
            ]
        ],
        "return": [
            [
                1,
                0,
                0,
                0
            ],
            [
                2,
                7,
                0,
                0
            ],
            [
                3,
                6,
                6,
                0
            ],
            [
                4,
                5,
                5,
                4
            ]
        ]
    },
    {
        "args": [
            [
                [
                    5,
                    7
                ],
                [
                    7,
                    9
                ]
            ]
        ],
        "return": [
            [
                5,
                0
            ],
            [
                7,
                9
            ]
        ]
    }
]
```
## Credits

Found on Edabit: [The Bottom of the Matrix](https://edabit.com/challenge/SqbyWYwqChQroXfhu)
