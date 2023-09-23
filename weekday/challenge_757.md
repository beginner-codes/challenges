# Challenge 757 - Find Value in a Binary Tree

A list that represents a Binary Tree is in the following form:
```python
binary_tree = [value, right, right]
```
When `left` is the left side of the tree and `right` is the right side of the tree.

To illustrate:
```javascript
tree1 = [
    3,
    [
        8,
        [
            5,
            null,
            null
        ],
        null
    ],
    [
        7,
        null,
        null
    ]
]
```
# list1 represents the following Binary Tree:
```
                    3
                   / \
                  8   7
                 / \ / \
                5  N N  N
               / \
              N   N

# While N represents null.
```
Create a function that takes a list that represent a Binary Tree and a value and return `True` if the value is in the tree and, `False` otherwise.

## Examples
```python
is_val_in_tree(tree1, 5) ➞ True

is_val_in_tree(tree1, 9) ➞ False

is_val_in_tree(tree2, 51) ➞ False
```
## Notes

- The tree will contain integers or `null` and will be presented by a list in the specified format.

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


def is_val_in_tree(tree: int, search: int) -> bool:
    return False  # Put your code here!!!


test(757, is_val_in_tree)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                3,
                [
                    7,
                    [
                        1,
                        null,
                        null
                    ],
                    [
                        8,
                        null,
                        null
                    ]
                ],
                [
                    5,
                    null,
                    [
                        4,
                        null,
                        null
                    ]
                ]
            ],
            15
        ],
        "return": false
    },
    {
        "args": [
            [
                3,
                [
                    7,
                    [
                        1,
                        null,
                        null
                    ],
                    [
                        8,
                        null,
                        null
                    ]
                ],
                [
                    5,
                    null,
                    [
                        4,
                        null,
                        null
                    ]
                ]
            ],
            7
        ],
        "return": true
    },
    {
        "args": [
            [
                9,
                [
                    15,
                    [
                        10,
                        null,
                        [
                            12,
                            null,
                            [
                                4,
                                [
                                    2,
                                    null,
                                    null
                                ],
                                null
                            ]
                        ]
                    ],
                    null
                ],
                [
                    6,
                    [
                        24,
                        null,
                        null
                    ],
                    [
                        18,
                        null,
                        null
                    ]
                ]
            ],
            23
        ],
        "return": false
    },
    {
        "args": [
            [
                9,
                [
                    15,
                    [
                        10,
                        null,
                        [
                            12,
                            null,
                            [
                                4,
                                [
                                    2,
                                    null,
                                    null
                                ],
                                null
                            ]
                        ]
                    ],
                    null
                ],
                [
                    6,
                    [
                        24,
                        null,
                        null
                    ],
                    [
                        18,
                        null,
                        null
                    ]
                ]
            ],
            51
        ],
        "return": false
    },
    {
        "args": [
            [
                9,
                [
                    15,
                    [
                        10,
                        null,
                        [
                            12,
                            null,
                            [
                                4,
                                [
                                    2,
                                    null,
                                    null
                                ],
                                null
                            ]
                        ]
                    ],
                    null
                ],
                [
                    6,
                    [
                        24,
                        null,
                        null
                    ],
                    [
                        18,
                        null,
                        null
                    ]
                ]
            ],
            18
        ],
        "return": true
    }
]
```

## Credits

Found on Edabit: [Find Value in a Binary Tree](https://edabit.com/challenge/KZFEAv8Sqh9zW5eLS)
