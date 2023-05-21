# Challenge 668 - Diagonal Domination

A square matrix (same number of rows as columns) is called row diagonally dominant if "the absolute value of each entry in the main diagonal is strictly larger than the sum of the absolute values of the other entries in that row".

**To illustrate ...**
```json
[
  [10, 3, 6],
  [2, -9, -6],
  [1, -1, 4]
]
```
The absolute values from top left to bottom right are:

10 = First item of first row.
9 = Second item of second row.
4 = Third item of third row.
... making a row diagonal dominant total of 23.

**In the first row ...**

The value of the row diagonal dominant is 10.
The sum of the other absolute values are 3 and 6 make a total of 9.
... so far, the matrix is row diagonally dominant, since 10 > 9.

**In the second row ...**

The value of the row diagonal dominant is 9.
The sum of the other absolute values in the second row are 3 and 6 which make a total of 9.
... meaning the matrix is not row diagonally dominant since 9 <= 9.
```json
[
  [10, 3, 6],
  [3, -9, -6],
  [1, -1,  4]
]
```
For a square to be row diagonally dominant, all the rows in the square have to be like Row 1.

Write a function that determines if a given square matrix is row diagonally dominant.

## Examples
```python
diag_dom([
  [2, -1],
  [-1, 2]
]) ➞ True

diag_dom([
  [0, 1],
  [1, 0]
]) ➞ False

diag_dom([
  [10, 3, 6],
  [2, -9, -6],
  [1, -1, 4]
]) ➞ True

diag_dom([
  [10, 3, 6],
  [4, -9, -6],
  [1, -1, 4]
]) ➞ False
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def diag_dom(matrix: list[list[int]]) -> bool:
    return False  # Put your code here!!!


test(668, diag_dom)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                [
                    0,
                    1
                ],
                [
                    1,
                    0
                ]
            ]
        ],
        "return": false
    },
    {
        "args": [
            [
                [
                    2,
                    -1
                ],
                [
                    -1,
                    2
                ]
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                [
                    5,
                    0,
                    -1,
                    0
                ],
                [
                    0,
                    -6,
                    0,
                    2
                ],
                [
                    3,
                    0,
                    7,
                    0
                ],
                [
                    0,
                    4,
                    0,
                    -8
                ]
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                [
                    10,
                    3,
                    6
                ],
                [
                    3,
                    -9,
                    -6
                ],
                [
                    1,
                    -1,
                    4
                ]
            ]
        ],
        "return": false
    },
    {
        "args": [
            [
                [
                    10,
                    3,
                    6
                ],
                [
                    2,
                    -9,
                    -6
                ],
                [
                    1,
                    -1,
                    4
                ]
            ]
        ],
        "return": true
    }
]

```
## Credits

Found on Edabit: [Diagonal Domination](https://edabit.com/challenge/5WvxKLK55JvT8NLfR)
