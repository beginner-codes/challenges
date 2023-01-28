# Challenge 596 - Three Sum Problem

Write a function that returns all sets of three elements that sum to `0`.

## Examples
```python
three_sum([0, 1, -1, -1, 2]) ➞ [[0, 1, -1], [-1, -1, 2]]

three_sum([0, 0, 0, 5, -5]) ➞ [[0, 0, 0], [0, 5, -5]]

three_sum([1, 2, 3]) ➞ []

three_sum([1]) ➞ []
```
## Notes

- The original list may contain duplicate numbers.
- Each three-element sublist in your output should be distinct.
- Sublists should be ordered by the first element of the sublist.
- Sublists themselves should be ordered the same as the original list.
- Return an empty list if no three elements sum to zero.
- Return an empty list if there are fewer than three elements.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def three_sum(numbers: list[int]) -> list[list[int]]:
    return []  # Put your code here!!!


test(596, three_sum)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                1,
                5,
                5,
                2
            ]
        ],
        "return": []
    },
    {
        "args": [
            []
        ],
        "return": []
    },
    {
        "args": [
            [
                0,
                -1,
                1,
                0,
                -1,
                1
            ]
        ],
        "return": [
            [
                0,
                -1,
                1
            ],
            [
                0,
                1,
                -1
            ],
            [
                -1,
                1,
                0
            ],
            [
                -1,
                0,
                1
            ],
            [
                1,
                0,
                -1
            ]
        ]
    },
    {
        "args": [
            [
                0,
                0,
                0,
                5,
                -5
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
                5,
                -5
            ]
        ]
    },
    {
        "args": [
            [
                0,
                5,
                -5,
                0,
                0
            ]
        ],
        "return": [
            [
                0,
                5,
                -5
            ],
            [
                0,
                0,
                0
            ],
            [
                5,
                -5,
                0
            ]
        ]
    },
    {
        "args": [
            [
                0,
                5,
                5,
                0,
                0
            ]
        ],
        "return": [
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
                1,
                2,
                3,
                -5,
                8,
                9,
                -9,
                0
            ]
        ],
        "return": [
            [
                1,
                8,
                -9
            ],
            [
                2,
                3,
                -5
            ],
            [
                9,
                -9,
                0
            ]
        ]
    },
    {
        "args": [
            [
                1,
                1
            ]
        ],
        "return": []
    },
    {
        "args": [
            [
                0,
                1,
                -1,
                -1,
                2
            ]
        ],
        "return": [
            [
                0,
                1,
                -1
            ],
            [
                -1,
                -1,
                2
            ]
        ]
    },
    {
        "args": [
            [
                0,
                0,
                0
            ]
        ],
        "return": [
            [
                0,
                0,
                0
            ]
        ]
    }
]
```
## Credits

Found on Edabit: [Three Sum Problem](https://edabit.com/challenge/gbybFzt2tLa5zfpHc)
