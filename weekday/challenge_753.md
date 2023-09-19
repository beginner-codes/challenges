# Challenge 753 - Sum of the Items in a List

Create a function that takes a list and returns the sum of all the items in that list.

## Examples
```python
sum_list([1, 2, 3]) ➞ 6
# 1 + 2 + 3 = 6

sum_list([1, [2, [1]], 3]) ➞ 7
# 1 + 2 + 1 + 3 = 7
```
## Notes

- An item in the list can be another list.

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
from typing import TypeAlias


NestedIntLists = "list[int | NestedIntLists]"


def sum_list(lists: NestedIntLists) -> int:
    return 0  # Put your code here!!!


test(753, sum_list)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                1,
                [
                    2,
                    [
                        1
                    ]
                ],
                3
            ]
        ],
        "return": 7
    },
    {
        "args": [
            [
                1,
                2,
                3
            ]
        ],
        "return": 6
    },
    {
        "args": [
            [
                1,
                [
                    1,
                    2
                ],
                [
                    3,
                    1
                ]
            ]
        ],
        "return": 8
    },
    {
        "args": [
            [
                [
                    1,
                    1
                ],
                [
                    2,
                    8
                ],
                8
            ]
        ],
        "return": 20
    },
    {
        "args": [
            [
                1,
                2
            ]
        ],
        "return": 3
    }
]
```

## Credits

Found on Edabit: [Sum of the Items in a List](https://edabit.com/challenge/pyMScvcjbxG7rMcNT)
