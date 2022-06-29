# Challenge 487 - Return a List of Sublists

Write a function that takes three arguments and returns a list containing sublists (e.g. `[[], [], []]`), each containing a given number of an item.

- `x` Number of sublists contained within the main list.
- `y` Number of items contained within each sublist.
- `z` Item contained within each sublist.

## Examples
```python
matrix(3, 2, 3) ➞ [[3, 3], [3, 3], [3, 3]]

matrix(2, 1, "beginner.codes") ➞ [["beginner.codes"], ["beginner.codes"]]

matrix(3, 2, 0) ➞ [[0, 0], [0, 0], [0, 0]]
```
## Notes

- The first two arguments will always be integers.
- The third argument is either a string or an integer.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test
from typing import TypeVar

T = TypeVar("T")

def matrix(x: int, y: int, z: int | str) -> list[list[int | str]]:
    return []  # Put your code here!!!


test(487, matrix)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            3,
            4,
            0
        ],
        "return": [
            [
                0,
                0,
                0,
                0
            ],
            [
                0,
                0,
                0,
                0
            ],
            [
                0,
                0,
                0,
                0
            ]
        ]
    },
    {
        "args": [
            2,
            3,
            "#"
        ],
        "return": [
            [
                "#",
                "#",
                "#"
            ],
            [
                "#",
                "#",
                "#"
            ]
        ]
    },
    {
        "args": [
            2,
            3,
            -4
        ],
        "return": [
            [
                -4,
                -4,
                -4
            ],
            [
                -4,
                -4,
                -4
            ]
        ]
    },
    {
        "args": [
            1,
            2,
            0
        ],
        "return": [
            [
                0,
                0
            ]
        ]
    }
]
```
## Credits

Found on Edabit: [Return a List of Sublists](https://edabit.com/challenge/9szPm9Mg5D2vJyTvf)
