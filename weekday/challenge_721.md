# Challenge 721 - Divide Array into Chunks

Write a function that divides a list into chunks of a given size.

## Examples
```python
chunkify([2, 3, 4, 5], 2) ➞ [[2, 3], [4, 5]]

chunkify([2, 3, 4, 5, 6], 2) ➞ [[2, 3], [4, 5], [6]]

chunkify([2, 3, 4, 5, 6, 7], 3) ➞ [[2, 3, 4], [5, 6, 7]]

chunkify([2, 3, 4, 5, 6, 7], 1) ➞ [[2], [3], [4], [5], [6], [7]]

chunkify([2, 3, 4, 5, 6, 7], 7) ➞ [[2, 3, 4, 5, 6, 7]]
```
## Notes

- It's ok if the last chunk is not completely filled.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def chunkify(numbers: list[str], chunk_size: int) -> list[list[int]]:
    return []  # Put your code here!!!


test(721, chunkify)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                2,
                3,
                4,
                5,
                6,
                7
            ],
            7
        ],
        "return": [
            [
                2,
                3,
                4,
                5,
                6,
                7
            ]
        ]
    },
    {
        "args": [
            [
                2,
                3,
                4,
                5,
                6,
                7,
                8
            ],
            3
        ],
        "return": [
            [
                2,
                3,
                4
            ],
            [
                5,
                6,
                7
            ],
            [
                8
            ]
        ]
    },
    {
        "args": [
            [
                2,
                3,
                4,
                5,
                6,
                7
            ],
            1
        ],
        "return": [
            [
                2
            ],
            [
                3
            ],
            [
                4
            ],
            [
                5
            ],
            [
                6
            ],
            [
                7
            ]
        ]
    },
    {
        "args": [
            [
                2,
                3,
                4,
                5
            ],
            2
        ],
        "return": [
            [
                2,
                3
            ],
            [
                4,
                5
            ]
        ]
    },
    {
        "args": [
            [
                2,
                3,
                4,
                5,
                6,
                7
            ],
            3
        ],
        "return": [
            [
                2,
                3,
                4
            ],
            [
                5,
                6,
                7
            ]
        ]
    }
]
```
## Credits

Found on Edabit: [Divide Array into Chunks](https://edabit.com/challenge/biJPWHr486Y4cPLnD)
