# Challenge 594 - Multiplicity of Numbers

Write a function that returns a list of elements `[number, multiplicity]`. The multiplicity of a number refers to the number of times it occurs in the provided list.

To illustrate:
```python
[5, 5, 1, 1, 5, 5, 3]
[[5, 4], [1, 2], [3, 1]]

# Since 5 appears 4 times, 1 appears twice, and 3 appearance once.
```
The final list should only include unique elements, and the elements should be ordered by when they first appeared in the original list.

## Examples
```python
multiplicity([1, 1, 1, 2, 2, 3]) ➞ [[1, 3], [2, 2], [3, 1]]

multiplicity([1, 1, 1, 1, 1]) ➞ [[1, 5]]

multiplicity([1, 5, 4, 3, 2]) ➞ [[1, 1], [5, 1], [4, 1], [3, 1], [2, 1]]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def multiplicity(numbers: list[int]) -> list[list[int]]:
    return []  # Put your code here!!!


test(594, multiplicity)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                5,
                5,
                5,
                5,
                8
            ]
        ],
        "return": [
            [
                5,
                4
            ],
            [
                8,
                1
            ]
        ]
    },
    {
        "args": [
            [
                3,
                3,
                3,
                0
            ]
        ],
        "return": [
            [
                3,
                3
            ],
            [
                0,
                1
            ]
        ]
    },
    {
        "args": [
            [
                1,
                1,
                2,
                2,
                3,
                3,
                4,
                4
            ]
        ],
        "return": [
            [
                1,
                2
            ],
            [
                2,
                2
            ],
            [
                3,
                2
            ],
            [
                4,
                2
            ]
        ]
    }
]
```
## Credits

Found on Edabit: [Multiplicity of Numbers](https://edabit.com/challenge/w5eFnzhADpLZSuCM3)
