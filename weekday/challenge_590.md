# Challenge 590 - Minesweeper Number of Neighbouring Mines

Create a function that takes a list representation of a Minesweeper board, and returns another board where the value of each cell is the number of neighbouring mines.

## Examples

The input may look like this:
```python
[
  [0, 1, 0, 0],
  [0, 0, 1, 0],
  [0, 1, 0, 1],
  [1, 1, 0, 0]
]
```
The `0` represents an empty space . The `1` represents a mine.

You will have to replace each mine with a `9` and each empty space with the number of adjacent mines, the output will look like this:
```python
[
  [1, 9, 2, 1],
  [2, 3, 9, 2],
  [3, 9, 4, 9],
  [9, 9, 3, 1]
]
```
## Notes

- Since in the output the numbers `0`-`8` are used to determine the amount of adjacent mines, the number `9` will be used to identify the mines instead.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def count_mines(board: list[list[int]]) -> list[list[int]]:
    return []  # Put your code here!!!


test(590, count_mines)  # Tell it which challenge to test against
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
                    1,
                    0,
                    0
                ],
                [
                    1,
                    0,
                    0,
                    0
                ],
                [
                    0,
                    0,
                    1,
                    0
                ]
            ]
        ],
        "return": [
            [
                1,
                1,
                2,
                9
            ],
            [
                2,
                9,
                2,
                1
            ],
            [
                9,
                3,
                2,
                1
            ],
            [
                1,
                2,
                9,
                1
            ]
        ]
    },
    {
        "args": [
            [
                [
                    1,
                    0,
                    0,
                    0,
                    0,
                    0,
                    1,
                    0
                ],
                [
                    1,
                    0,
                    1,
                    0,
                    1,
                    0,
                    0,
                    0
                ],
                [
                    0,
                    0,
                    0,
                    0,
                    0,
                    0,
                    1,
                    0
                ],
                [
                    0,
                    1,
                    0,
                    1,
                    0,
                    0,
                    0,
                    1
                ],
                [
                    0,
                    0,
                    0,
                    1,
                    0,
                    1,
                    1,
                    0
                ],
                [
                    0,
                    1,
                    1,
                    0,
                    0,
                    0,
                    1,
                    1
                ],
                [
                    1,
                    0,
                    0,
                    0,
                    0,
                    0,
                    0,
                    0
                ],
                [
                    0,
                    0,
                    1,
                    0,
                    0,
                    1,
                    0,
                    1
                ]
            ]
        ],
        "return": [
            [
                9,
                3,
                1,
                2,
                1,
                2,
                9,
                1
            ],
            [
                9,
                3,
                9,
                2,
                9,
                3,
                2,
                2
            ],
            [
                2,
                3,
                3,
                3,
                2,
                2,
                9,
                2
            ],
            [
                1,
                9,
                3,
                9,
                3,
                3,
                4,
                9
            ],
            [
                2,
                3,
                5,
                9,
                3,
                9,
                9,
                4
            ],
            [
                2,
                9,
                9,
                2,
                2,
                3,
                9,
                9
            ],
            [
                9,
                4,
                3,
                2,
                1,
                2,
                4,
                3
            ],
            [
                1,
                2,
                9,
                1,
                1,
                9,
                2,
                9
            ]
        ]
    },
    {
        "args": [
            []
        ],
        "return": []
    }
]
```
## Credits

Found on Edabit: [Minesweeper Number of Neighbouring Mines](https://edabit.com/challenge/v2eHXTn2qobw2WYJP)
