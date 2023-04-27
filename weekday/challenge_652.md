# Challenge 652 - An Ordered Matrix!

Create an ordered 2D list (matrix). A matrix is ordered if its `(0, 0)` element is `1`, its `(0, 1)` element is `2`, and so on. Your function needs to create an `a × b` matrix. `a` is the first argument and `b` is the second.

## Examples
```python
ordered_matrix(5, 5) ➞ [
  [1, 2, 3, 4, 5],
  [6, 7, 8, 9, 10],
  [11, 12, 13, 14, 15],
  [16, 17, 18, 19, 20],
  [21, 22, 23, 24, 25]
]

ordered_matrix(1, 1) ➞ [[1]]

ordered_matrix(1, 5) ➞ [[1, 2, 3, 4, 5]]
```
## Notes

- `a` is the height of the matrix (`y` coordinate), and `b` is the width (`x` coordinate).
- `a` and `b` will always be positive, and the matrix will always be square shaped (in each row are the same amount of columns).
- `a` and `b` are integers.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def ordered_matrix(a: int, b: int) -> list[list[int]]:
    return []  # Put your code here!!!


test(652, ordered_matrix)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            1,
            2
        ],
        "return": [
            [
                1,
                2
            ]
        ]
    },
    {
        "args": [
            3,
            4
        ],
        "return": [
            [
                1,
                2,
                3,
                4
            ],
            [
                5,
                6,
                7,
                8
            ],
            [
                9,
                10,
                11,
                12
            ]
        ]
    },
    {
        "args": [
            3,
            3
        ],
        "return": [
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
    },
    {
        "args": [
            5,
            5
        ],
        "return": [
            [
                1,
                2,
                3,
                4,
                5
            ],
            [
                6,
                7,
                8,
                9,
                10
            ],
            [
                11,
                12,
                13,
                14,
                15
            ],
            [
                16,
                17,
                18,
                19,
                20
            ],
            [
                21,
                22,
                23,
                24,
                25
            ]
        ]
    }
]
```
## Credits

Found on Edabit: [An Ordered Matrix](https://edabit.com/challenge/exeY2wDuEW4rFeYvL)
