# Challenge 467 - Concatenate to Form Target List

Create a function that returns `True` if the smaller lists can be concatenated to form the target list and `False` otherwise.

## Examples
```python
can_concatenate([[1, 2, 3, 4], [5, 6], [7]], [1, 2, 3, 4, 5, 6, 7]) ➞ True

can_concatenate([[2, 1, 3], [5, 4, 7, 6]], [7, 6, 5, 4, 3, 2, 1]) ➞ True

can_concatenate([[2, 1, 3], [5, 4, 7, 6, 7]], [1, 2, 3, 4, 5, 6, 7]) ➞ False
# Duplicate 7s not found in target list.

can_concatenate([[2, 1, 3], [5, 4, 7]], [1, 2, 3, 4, 5, 6, 7]) ➞ False
# Missing 6 from target list.
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from beginnercodes.challenges import test


def can_concatenate(lists: list[list[int]], target: list[int]) -> bool:
    return False  # Put your code here!!!


test(467, can_concatenate)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                [
                    1,
                    2,
                    3,
                    4
                ],
                [
                    5,
                    6
                ],
                [
                    7
                ]
            ],
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
        "return": true
    },
    {
        "args": [
            [
                [
                    2,
                    1,
                    3
                ],
                [
                    5,
                    4,
                    7,
                    6
                ]
            ],
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
        "return": true
    },
    {
        "args": [
            [
                [
                    2,
                    1,
                    3
                ],
                [
                    5,
                    4,
                    7,
                    6
                ]
            ],
            [
                7,
                6,
                5,
                4,
                3,
                2,
                1
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                [
                    2,
                    1,
                    3
                ],
                [
                    5,
                    4,
                    7,
                    6,
                    7
                ]
            ],
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
        "return": false
    },
    {
        "args": [
            [
                [
                    2,
                    1,
                    3
                ],
                [
                    5,
                    4,
                    7
                ]
            ],
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
        "return": false
    }
]
```
## Credits

Found on Edabit: [Concatenate to Form Target List](https://edabit.com/challenge/23htQEtZobC8cfwcm)
