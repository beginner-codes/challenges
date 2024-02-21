# Challenge 827 - Flip the Array

Create a function that flips a horizontal list into a vertical list, and a vertical list into a horizontal list.

In other words, take an `1 x n` list (1 row + `n` columns) and flip it into an `n x 1` list (`n` rows and 1 column), and vice versa.

## Examples
```python
flip_list([1, 2, 3, 4]) ➞ [[1], [2], [3], [4]]
# Take a horizontal list and flip it vertical.

flip_list([[5], [6], [9]]) ➞ [5, 6, 9]
# Take a vertical list and flip it horizontal.

flip_list([]) ➞ []
```
## Notes

- If given an empty list `[]`, return an empty list `[]`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. *
*[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a
key `args` that are a list of parameters your function should take. The `return` key is what your function should return
given the `args`.

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your
solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:

```python
from __future__ import annotations
from beginnercodes.challenges import test


def flip_list(lst: list[list | int]) -> list[list | int]:
    return []  # Put your code here!!!


test(827, flip_list)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                [
                    7
                ],
                [
                    8
                ],
                [
                    9
                ],
                [
                    55
                ]
            ]
        ],
        "return": [
            7,
            8,
            9,
            55
        ]
    },
    {
        "args": [
            [
                1,
                2,
                3,
                4
            ]
        ],
        "return": [
            [
                1
            ],
            [
                2
            ],
            [
                3
            ],
            [
                4
            ]
        ]
    },
    {
        "args": [
            [
                [
                    5
                ],
                [
                    6
                ],
                [
                    9
                ]
            ]
        ],
        "return": [
            5,
            6,
            9
        ]
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
                7,
                8,
                9,
                55
            ]
        ],
        "return": [
            [
                7
            ],
            [
                8
            ],
            [
                9
            ],
            [
                55
            ]
        ]
    }
]
```

## Credits

Found on Edabit: [Flip the Array](https://edabit.com/challenge/QoavwQhmrDpXJhBW9)
