# Challenge 714 - Multiplication Table

Create a function that takes an integer and returns multiplication table from 1 to the nth multiple.

## Examples
```python
multiplication_table(2) ➞ [
  [1, 2],
  [2, 4]
]

multiplication_table(3) ➞ [
  [1, 2, 3],
  [2, 4, 6],
  [3, 6, 9]
]

multiplication_table(5) ➞ [
  [1, 2, 3, 4, 5],
  [2, 4, 6, 8, 10],
  [3, 6, 9, 12, 15],
  [4, 8, 12, 16, 20],
  [5, 10, 15, 20, 25]
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


def multiplication_table(n: int) -> list[list[int]]:
    return []  # Put your code here!!!


test(714, multiplication_table)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            4
        ],
        "return": [
            [
                1,
                2,
                3,
                4
            ],
            [
                2,
                4,
                6,
                8
            ],
            [
                3,
                6,
                9,
                12
            ],
            [
                4,
                8,
                12,
                16
            ]
        ]
    },
    {
        "args": [
            1
        ],
        "return": [
            [
                1
            ]
        ]
    },
    {
        "args": [
            2
        ],
        "return": [
            [
                1,
                2
            ],
            [
                2,
                4
            ]
        ]
    },
    {
        "args": [
            5
        ],
        "return": [
            [
                1,
                2,
                3,
                4,
                5
            ],
            [
                2,
                4,
                6,
                8,
                10
            ],
            [
                3,
                6,
                9,
                12,
                15
            ],
            [
                4,
                8,
                12,
                16,
                20
            ],
            [
                5,
                10,
                15,
                20,
                25
            ]
        ]
    },
    {
        "args": [
            3
        ],
        "return": [
            [
                1,
                2,
                3
            ],
            [
                2,
                4,
                6
            ],
            [
                3,
                6,
                9
            ]
        ]
    }
]
```
## Credits

Found on Edabit: [Multiplication Table](https://edabit.com/challenge/mrKbfWBjQA2c3amwN)
