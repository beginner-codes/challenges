# Challenge 465 - Deepest Sub-Array

You are given an array which may contain sub-arrays. Your task is to find the depth of the deepest sub-array.
```
[a] = 1 depth
[[a]] = 2 depth
[[[a]]] = 3 depth, etc
```
## Examples
```python
deepest([1, [2, 3], 4, [5, 6]]) ➞ 2

deepest([[[[[[[[[[1]]]]]]]]]]) ➞ 10

deepest([1, 4, [1, 4, [1, 4, [1, 4, [5]]]]]) ➞ 5
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from beginnercodes.challenges import test


def deepest(array: list) -> int:
    return 0  # Put your code here!!!


test(465, deepest)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                1,
                4,
                5
            ]
        ],
        "return": 1
    },
    {
        "args": [
            [
                [
                    2,
                    3
                ],
                4,
                [
                    6,
                    7,
                    [
                        8
                    ]
                ]
            ]
        ],
        "return": 3
    },
    {
        "args": [
            [
                5,
                [
                    [
                        [
                            [
                                [
                                    [
                                        [
                                            [
                                                [
                                                    [
                                                        2
                                                    ]
                                                ]
                                            ]
                                        ]
                                    ]
                                ]
                            ]
                        ]
                    ]
                ],
                [
                    [
                        [
                            [
                                [
                                    [
                                        [
                                            [
                                                [
                                                    [
                                                        [
                                                            [
                                                                4
                                                            ]
                                                        ]
                                                    ]
                                                ]
                                            ]
                                        ]
                                    ]
                                ]
                            ]
                        ]
                    ]
                ]
            ]
        ],
        "return": 13
    },
    {
        "args": [
            [
                [
                    [
                        3,
                        2,
                        [
                            [
                                4
                            ]
                        ],
                        8
                    ],
                    [
                        [
                            2,
                            4
                        ],
                        5
                    ]
                ],
                3,
                5,
                [
                    9,
                    1
                ]
            ]
        ],
        "return": 5
    },
    {
        "args": [
            [
                [
                    6,
                    9,
                    6
                ],
                [
                    [
                        [
                            1,
                            4
                        ],
                        0,
                        8
                    ],
                    [
                        8,
                        0,
                        [
                            4,
                            1
                        ]
                    ]
                ],
                [
                    [
                        5,
                        3,
                        4
                    ],
                    [
                        4,
                        3,
                        5
                    ]
                ]
            ]
        ],
        "return": 4
    }
]
```
## Credits

Found on Edabit: [Deepest Sublist](https://edabit.com/challenge/iLLqX4nC2HT2xxg3F)
