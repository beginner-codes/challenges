# Challenge 523 - Is it a Probability Matrix? 

In probability theory, a probability matrix is a matrix such that:

- The matrix is a square matrix (same number of rows as columns).
- All entries are probabilities, i.e. numbers between 0 and 1.
- All rows add up to 1.
- 
The following is an example of a probability matrix:
```json
[
  [0.5, 0.5, 0.0],
  [0.2, 0.5, 0.3],
  [0.1, 0.2, 0.7]
]
```
Note that though all rows add up to 1, there is no restriction on the columns, which may or may not add up to 1.

Write a function that determines if a matrix is a probability matrix or not.

## Examples
```python
is_prob_matrix([
  [0.5, 0.5, 0.0],
  [0.2, 0.5, 0.3],
  [0.1, 0.2, 0.7]
]) ➞ True

is_prob_matrix([
  [0.5, 0.5, 0.0],
  [0.2, 0.5, 0.3]
]) ➞ False

# Not a square matrix.

is_prob_matrix([
  [2, -1],
  [-1, 2]
]) ➞ False

# Entries not between 0 and 1.

is_prob_matrix([
  [0, 1],
  [1, 0]
]) ➞ True

is_prob_matrix([
  [0.5, 0.4],
  [0.5, 0.6]
]) ➞ False

# Rows do not add to 1.
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def is_prob_matrix(matrix: list[list[float]]) -> bool:
    return False # Put your code here!!!


test(523, is_prob_matrix)  # Tell it which challenge to test against
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
                    0,
                    1
                ],
                [
                    0,
                    0,
                    0,
                    1
                ],
                [
                    0,
                    0,
                    0,
                    1
                ],
                [
                    0,
                    0,
                    0,
                    1
                ]
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                [
                    0.5,
                    0.0,
                    0.5,
                    0.0
                ],
                [
                    0.1,
                    0.2,
                    0.3,
                    0.4
                ],
                [
                    0.3,
                    0.2,
                    0.2,
                    0.3
                ],
                [
                    0.0,
                    0.5,
                    0.0,
                    0.5
                ]
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                [
                    2,
                    1
                ],
                [
                    1,
                    2
                ]
            ]
        ],
        "return": false
    },
    {
        "args": [
            [
                [
                    1
                ]
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                [
                    0.5,
                    0.4
                ],
                [
                    0.5,
                    0.6
                ]
            ]
        ],
        "return": false
    }
]
```
## Credits

Found on Edabit: [Is it a Probability Matrix?](https://edabit.com/challenge/TJHwPqtA7DRGKJitB)
