# Challenge 504 - Minesweeper Grid

This challenge is based on the game Minesweeper.

Create a function that takes a grid of `#` and `-`, where each hash (`#`) represents a mine and each dash (`-`) represents a mine-free spot. Return a list where each dash is replaced by a digit indicating the number of mines immediately adjacent to the spot (horizontally, vertically, and diagonally).

## Examples
```python
num_grid([
  ["-", "-", "-", "-", "-"],
  ["-", "-", "-", "-", "-"],
  ["-", "-", "#", "-", "-"],
  ["-", "-", "-", "-", "-"],
  ["-", "-", "-", "-", "-"]
]) ➞ [
  ["0", "0", "0", "0", "0"],
  ["0", "1", "1", "1", "0"],
  ["0", "1", "#", "1", "0"],
  ["0", "1", "1", "1", "0"],
  ["0", "0", "0", "0", "0"],
]

num_grid([
  ["-", "-", "-", "-", "#"],
  ["-", "-", "-", "-", "-"],
  ["-", "-", "#", "-", "-"],
  ["-", "-", "-", "-", "-"],
  ["#", "-", "-", "-", "-"]
]) ➞ [
  ["0", "0", "0", "1", "#"],
  ["0", "1", "1", "2", "1"],
  ["0", "1", "#", "1", "0"],
  ["1", "2", "1", "1", "0"],
  ["#", "1", "0", "0", "0"]
]

num_grid([
  ["-", "-", "-", "#", "#"],
  ["-", "#", "-", "-", "-"],
  ["-", "-", "#", "-", "-"],
  ["-", "#", "#", "-", "-"],
  ["-", "-", "-", "-", "-"]
]) ➞ [
  ["1", "1", "2", "#", "#"],
  ["1", "#", "3", "3", "2"],
  ["2", "4", "#", "2", "0"],
  ["1", "#", "#", "2", "0"],
  ["1", "2", "2", "1", "0"],
]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def wiggle_string(string: str) -> list[str]:
    return []  # Put your code here!!!


test(503, wiggle_string)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                [
                    "-",
                    "-",
                    "-",
                    "-",
                    "-"
                ],
                [
                    "-",
                    "-",
                    "-",
                    "-",
                    "-"
                ],
                [
                    "-",
                    "-",
                    "#",
                    "-",
                    "-"
                ],
                [
                    "-",
                    "-",
                    "-",
                    "-",
                    "-"
                ],
                [
                    "-",
                    "-",
                    "-",
                    "-",
                    "-"
                ]
            ]
        ],
        "return": [
            [
                "0",
                "0",
                "0",
                "0",
                "0"
            ],
            [
                "0",
                "1",
                "1",
                "1",
                "0"
            ],
            [
                "0",
                "1",
                "#",
                "1",
                "0"
            ],
            [
                "0",
                "1",
                "1",
                "1",
                "0"
            ],
            [
                "0",
                "0",
                "0",
                "0",
                "0"
            ]
        ]
    },
    {
        "args": [
            [
                [
                    "-",
                    "-",
                    "-",
                    "-",
                    "#"
                ],
                [
                    "-",
                    "-",
                    "-",
                    "-",
                    "-"
                ],
                [
                    "-",
                    "-",
                    "#",
                    "-",
                    "-"
                ],
                [
                    "-",
                    "-",
                    "-",
                    "-",
                    "-"
                ],
                [
                    "#",
                    "-",
                    "-",
                    "-",
                    "-"
                ]
            ]
        ],
        "return": [
            [
                "0",
                "0",
                "0",
                "1",
                "#"
            ],
            [
                "0",
                "1",
                "1",
                "2",
                "1"
            ],
            [
                "0",
                "1",
                "#",
                "1",
                "0"
            ],
            [
                "1",
                "2",
                "1",
                "1",
                "0"
            ],
            [
                "#",
                "1",
                "0",
                "0",
                "0"
            ]
        ]
    },
    {
        "args": [
            [
                [
                    "-",
                    "-",
                    "-",
                    "#",
                    "#"
                ],
                [
                    "-",
                    "#",
                    "-",
                    "-",
                    "-"
                ],
                [
                    "-",
                    "-",
                    "#",
                    "-",
                    "-"
                ],
                [
                    "-",
                    "#",
                    "#",
                    "-",
                    "-"
                ],
                [
                    "-",
                    "-",
                    "-",
                    "-",
                    "-"
                ]
            ]
        ],
        "return": [
            [
                "1",
                "1",
                "2",
                "#",
                "#"
            ],
            [
                "1",
                "#",
                "3",
                "3",
                "2"
            ],
            [
                "2",
                "4",
                "#",
                "2",
                "0"
            ],
            [
                "1",
                "#",
                "#",
                "2",
                "0"
            ],
            [
                "1",
                "2",
                "2",
                "1",
                "0"
            ]
        ]
    }
]
```
## Credits

Found on Edabit: [Minesweeper I — Grid](https://edabit.com/challenge/YDgtdP69Mn9pC73xN)
