# Challenge 513 - Advanced List Sort

Create a function that takes a list of numbers or strings and returns a list with the items from the original list stored into sublists. Items of the same value should be in the same sublist.

## Examples
```python
advanced_sort([2, 1, 2, 1]) ➞ [[2, 2], [1, 1]]

advanced_sort([5, 4, 5, 5, 4, 3]) ➞ [[5, 5, 5], [4, 4], [3]]

advanced_sort(["b", "a", "b", "a", "c"]) ➞ [["b", "b"], ["a", "a"], ["c"]]
```
## Notes

- The sublists should be returned in the order of each element's first appearance in the given list.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from typing import TypeVar
from beginnercodes.challenges import test


T = TypeVar("T")


def advanced_sort(items: list[T]) -> list[list[T]]:
    return [] # Put your code here!!!


test(513, advanced_sort)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                1,
                2,
                1,
                2
            ]
        ],
        "return": [
            [
                1,
                1
            ],
            [
                2,
                2
            ]
        ]
    },
    {
        "args": [
            [
                5,
                5,
                4,
                3,
                4,
                4
            ]
        ],
        "return": [
            [
                5,
                5
            ],
            [
                4,
                4,
                4
            ],
            [
                3
            ]
        ]
    },
    {
        "args": [
            [
                80,
                80,
                4,
                60,
                60,
                3
            ]
        ],
        "return": [
            [
                80,
                80
            ],
            [
                4
            ],
            [
                60,
                60
            ],
            [
                3
            ]
        ]
    },
    {
        "args": [
            [
                3,
                2,
                1,
                3,
                2,
                1
            ]
        ],
        "return": [
            [
                3,
                3
            ],
            [
                2,
                2
            ],
            [
                1,
                1
            ]
        ]
    },
    {
        "args": [
            [
                "c",
                "c",
                "b",
                "c",
                "b",
                1,
                1
            ]
        ],
        "return": [
            [
                "c",
                "c",
                "c"
            ],
            [
                "b",
                "b"
            ],
            [
                1,
                1
            ]
        ]
    }
]
```
## Credits

Found on Edabit: [Advanced List Sort](https://edabit.com/challenge/6vSZmN66xhMRDX8YT)
