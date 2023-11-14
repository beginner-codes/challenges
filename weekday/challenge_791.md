# Challenge 791 - Matrix Subtraction

Two matrices must have an equal number of rows and columns to be subtracted. In which case, the subtraction of two matrices results in a matrix with the same number of rows and columns.

The result of the subtraction of A and B is computed by subtracting the corresponding elements of A and B.

Create a function that takes two matrices and returns that matrix that is their difference.

## Examples
```python
subtract_matrix([
  [1, 2, 3],
  [4, 5, 6],
  [7, 8, 9]
], [
  [1, 2, 3],
  [4, 5, 6],
  [7, 8, 9]
]) ➞ [
  [0, 0, 0],
  [0, 0, 0],
  [0, 0, 0]
]
```
## Notes

- If the matrices cannot be subtracted return an empty list

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


def subtract_matrix(matrix_a: list[list[int | float]], matrix: list[list[int | float]]) -> list[list[int | float]]:
    return []  # Put your code here!!!


test(791, subtract_matrix)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                [
                    0,
                    0,
                    0
                ],
                [
                    0,
                    0,
                    0
                ],
                [
                    0,
                    0,
                    0
                ]
            ],
            [
                [
                    0,
                    0,
                    0
                ],
                [
                    0,
                    0,
                    0
                ],
                [
                    0,
                    0,
                    0
                ]
            ]
        ],
        "return": [
            [
                0,
                0,
                0
            ],
            [
                0,
                0,
                0
            ],
            [
                0,
                0,
                0
            ]
        ]
    },
    {
        "args": [
            [
                [
                    21
                ]
            ],
            [
                [
                    63
                ]
            ]
        ],
        "return": [
            [
                -42
            ]
        ]
    },
    {
        "args": [
            [
                [
                    1,
                    2
                ],
                [
                    4,
                    5
                ]
            ],
            [
                [
                    1,
                    2
                ],
                [
                    4,
                    5
                ]
            ]
        ],
        "return": [
            [
                0,
                0
            ],
            [
                0,
                0
            ]
        ]
    },
    {
        "args": [
            [
                [
                    1,
                    2
                ],
                [
                    4,
                    -5
                ]
            ],
            [
                [
                    2,
                    2
                ],
                [
                    4,
                    -5
                ]
            ]
        ],
        "return": [
            [
                -1,
                0
            ],
            [
                0,
                0
            ]
        ]
    },
    {
        "args": [
            [
                [
                    1
                ]
            ],
            [
                [
                    1,
                    2
                ]
            ]
        ],
        "return": []
    }
]
```

## Credits

Found on Edabit: [Matrix Subtraction](https://edabit.com/challenge/DC2s6hM8yE7RvBr3S)
