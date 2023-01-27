# Challenge 595 - A Simple Dance

You will be given a list of dancing couples, with the woman first and man second, as well as a parameter `"men"` or `"women"`.

- If the parameter is `"men"`, the men reverse their positions (first moves to last, last moves to first, etc.), while women keep their positions.
- If the parameter is `"women"`, the women reverse their positions, while men keep their positions.

## Examples
```python
dance([
  ["Ana", "Bob"],
  ["Amy", "Josh"],
  ["Lisa", "Tim"]
], "men") ➞ [
  ["Ana", "Tim"],
  ["Amy", "Josh"],
  ["Lisa", "Bob"]
]

dance([
  ["Ana", "Bob"],
  ["Amy", "Josh"],
  ["Lisa", "Tim"]
], "women") ➞ [
  ["Lisa", "Bob"],
  ["Amy", "Josh"],
  ["Ana", "Tim"]
]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def dance(dancers: list[list[str]]) -> list[list[str]]:
    return []  # Put your code here!!!


test(595, dance)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                [
                    "w1",
                    "m1"
                ],
                [
                    "w2",
                    "m2"
                ],
                [
                    "w3",
                    "m3"
                ],
                [
                    "w4",
                    "m4"
                ],
                [
                    "w5",
                    "m5"
                ],
                [
                    "w6",
                    "m6"
                ]
            ],
            "women"
        ],
        "return": [
            [
                "w6",
                "m1"
            ],
            [
                "w5",
                "m2"
            ],
            [
                "w4",
                "m3"
            ],
            [
                "w3",
                "m4"
            ],
            [
                "w2",
                "m5"
            ],
            [
                "w1",
                "m6"
            ]
        ]
    },
    {
        "args": [
            [
                [
                    "Ana",
                    "Bob"
                ],
                [
                    "Amy",
                    "Josh"
                ],
                [
                    "Catty",
                    "Mark"
                ]
            ],
            "women"
        ],
        "return": [
            [
                "Catty",
                "Bob"
            ],
            [
                "Amy",
                "Josh"
            ],
            [
                "Ana",
                "Mark"
            ]
        ]
    },
    {
        "args": [
            [
                [
                    "w1",
                    "m1"
                ],
                [
                    "w2",
                    "m2"
                ],
                [
                    "w3",
                    "m3"
                ],
                [
                    "w4",
                    "m4"
                ],
                [
                    "w5",
                    "m5"
                ],
                [
                    "w6",
                    "m6"
                ]
            ],
            "men"
        ],
        "return": [
            [
                "w1",
                "m6"
            ],
            [
                "w2",
                "m5"
            ],
            [
                "w3",
                "m4"
            ],
            [
                "w4",
                "m3"
            ],
            [
                "w5",
                "m2"
            ],
            [
                "w6",
                "m1"
            ]
        ]
    },
    {
        "args": [
            [
                [
                    "Ana",
                    "Mark"
                ],
                [
                    "Lisa",
                    "John"
                ]
            ],
            "women"
        ],
        "return": [
            [
                "Lisa",
                "Mark"
            ],
            [
                "Ana",
                "John"
            ]
        ]
    },
    {
        "args": [
            [
                [
                    "Ana",
                    "Bob"
                ],
                [
                    "Amy",
                    "Josh"
                ],
                [
                    "Catty",
                    "Mark"
                ]
            ],
            "men"
        ],
        "return": [
            [
                "Ana",
                "Mark"
            ],
            [
                "Amy",
                "Josh"
            ],
            [
                "Catty",
                "Bob"
            ]
        ]
    }
]
```
## Credits

Found on Edabit: [A Simple Dance](https://edabit.com/challenge/8cJnRPxtjNP64k5fq)
