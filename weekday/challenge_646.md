# Challenge 646 - Beginning and End Pairs

Write a function that pairs the first number in an array with the last, the second number with the second to last, etc.

## Examples
```python
pairs([1, 2, 3, 4, 5, 6, 7]) ➞ [[1, 7], [2, 6], [3, 5], [4, 4]]

pairs([1, 2, 3, 4, 5, 6]) ➞ [[1, 6], [2, 5], [3, 4]]

pairs([5, 9, 8, 1, 2]) ➞ [[5, 2], [9, 1], [8, 8]]

pairs([]) ➞ []
```
## Notes

- If the list has an odd length, repeat the middle element twice for the last pair.
- Return an empty list if the input is an empty list.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def pairs(numbers: list[int]) -> list[list[int]]:
    return []  # Put your code here!!!


test(646, pairs)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                5,
                6
            ]
        ],
        "return": [
            [
                5,
                6
            ]
        ]
    },
    {
        "args": [
            [
                1,
                1,
                4,
                4,
                5,
                5
            ]
        ],
        "return": [
            [
                1,
                5
            ],
            [
                1,
                5
            ],
            [
                4,
                4
            ]
        ]
    },
    {
        "args": [
            [
                5,
                9,
                8,
                1,
                2
            ]
        ],
        "return": [
            [
                5,
                2
            ],
            [
                9,
                1
            ],
            [
                8,
                8
            ]
        ]
    },
    {
        "args": [
            [
                1,
                2,
                3,
                4,
                5,
                6,
                7
            ]
        ],
        "return": [
            [
                1,
                7
            ],
            [
                2,
                6
            ],
            [
                3,
                5
            ],
            [
                4,
                4
            ]
        ]
    },
    {
        "args": [
            [
                5,
                6,
                7
            ]
        ],
        "return": [
            [
                5,
                7
            ],
            [
                6,
                6
            ]
        ]
    }
]
```
## Credits

Found on Edabit: [Beginning and End Pairs](https://edabit.com/challenge/HrCuzAKE6skEYgDmf)
