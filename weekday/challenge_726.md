# Challenge 726 - Incrementing Rows and Columns

Write a function that takes in three parameters: a number of rows, a number of columns, and a series are increment operations and return the matrix that results from applying the +1 increment operations to a matrix initialized with zeros.

To illustrate:
```python
final(3, 3, ["2r", "2c", "1r", "0c"])

# Initialize a 3 x 3 matrix of zeroes.

[
  [0, 0, 0],
  [0, 0, 0],
  [0, 0, 0]
]

# Apply "2r" (increment index 2 row).

[
  [0, 0, 0],
  [0, 0, 0],
  [1, 1, 1]
]

# Apply "2c" (increment index 2 column).

[
  [0, 0, 1],
  [0, 0, 1],
  [1, 1, 2]
]

# Apply "1r" (increment index 1 row).

[
  [0, 0, 1],
  [1, 1, 2],
  [1, 1, 2]
]

# Apply "0c" (increment index 0 column).
# This is the result you should return.

[
  [1, 0, 1],
  [2, 1, 2],
  [2, 1, 2]
]
```
## Examples
```python
final(2, 2, ["0r", "0r", "0r", "1c"]) ➞ [
  [3, 4],
  [0, 1]
]

final(2, 2, ["0c"]) ➞ [
  [1, 0],
  [1, 0]
]

final(3, 3, ["1c", "2c", "2c", "3c", "3c", "3c"]) ➞ [
    [1, 2, 3],
    [1, 2, 3],
    [1, 2, 3]
]

final(3, 3, []) ➞ [
  [0, 0, 0],
  [0, 0, 0],
  [0, 0, 0]
]
```
## Notes

- The 2D matrix is 0-indexed.
- The matrix created will have at least one row and one column.
- All increment operations are +1.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def final(columns: int, rows: int, increments: list[str]) -> list[list[int]]:
    return []  # Put your code here!!!


test(726, final)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            2,
            2,
            [
                "0r",
                "0r",
                "0r",
                "1c"
            ]
        ],
        "return": [
            [
                3,
                4
            ],
            [
                0,
                1
            ]
        ]
    },
    {
        "args": [
            3,
            4,
            [
                "1r",
                "1r",
                "1r",
                "3c",
                "3c",
                "3c"
            ]
        ],
        "return": [
            [
                0,
                0,
                0,
                3
            ],
            [
                3,
                3,
                3,
                6
            ],
            [
                0,
                0,
                0,
                3
            ]
        ]
    },
    {
        "args": [
            1,
            1,
            []
        ],
        "return": [
            [
                0
            ]
        ]
    },
    {
        "args": [
            3,
            3,
            []
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
            3,
            3,
            [
                "2r",
                "2c",
                "1r",
                "0c"
            ]
        ],
        "return": [
            [
                1,
                0,
                1
            ],
            [
                2,
                1,
                2
            ],
            [
                2,
                1,
                2
            ]
        ]
    }
]
```
## Credits

Found on Edabit: [Incrementing Rows and Columns](https://edabit.com/challenge/8BQKa98d3s9Kis4vv)
