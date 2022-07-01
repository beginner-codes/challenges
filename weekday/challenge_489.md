# Challenge 489 - Diamond Shaped Array

Create a function that returns an array that expands by 1 from 1 to the value of the input, and then reduces back to 1. Items in the lists will be the same as the length of the lists.

## Examples
```python
diamond_arrays(1) ➞ [
    [1]
]

diamond_arrays(2) ➞ [
     [1], 
    [2, 2], 
     [1]
]

diamond_arrays(5) ➞ [
        [1],
       [2, 2],
      [3, 3, 3],
     [4, 4, 4, 4],
    [5, 5, 5, 5, 5],
     [4, 4, 4, 4],
      [3, 3, 3],
       [2, 2],
        [1]
]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def diamond_arrays(size: int) -> list[list[int]]:
    return []  # Put your code here!!!


test(489, diamond_arrays)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
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
                1
            ],
            [
                2,
                2
            ],
            [
                1
            ]
        ]
    },
    {
        "args": [
            3
        ],
        "return": [
            [
                1
            ],
            [
                2,
                2
            ],
            [
                3,
                3,
                3
            ],
            [
                2,
                2
            ],
            [
                1
            ]
        ]
    },
    {
        "args": [
            5
        ],
        "return": [
            [
                1
            ],
            [
                2,
                2
            ],
            [
                3,
                3,
                3
            ],
            [
                4,
                4,
                4,
                4
            ],
            [
                5,
                5,
                5,
                5,
                5
            ],
            [
                4,
                4,
                4,
                4
            ],
            [
                3,
                3,
                3
            ],
            [
                2,
                2
            ],
            [
                1
            ]
        ]
    },
    {
        "args": [
            7
        ],
        "return": [
            [
                1
            ],
            [
                2,
                2
            ],
            [
                3,
                3,
                3
            ],
            [
                4,
                4,
                4,
                4
            ],
            [
                5,
                5,
                5,
                5,
                5
            ],
            [
                6,
                6,
                6,
                6,
                6,
                6
            ],
            [
                7,
                7,
                7,
                7,
                7,
                7,
                7
            ],
            [
                6,
                6,
                6,
                6,
                6,
                6
            ],
            [
                5,
                5,
                5,
                5,
                5
            ],
            [
                4,
                4,
                4,
                4
            ],
            [
                3,
                3,
                3
            ],
            [
                2,
                2
            ],
            [
                1
            ]
        ]
    }
]

```
## Credits

Found on Edabit: [Diamond Shaped Array](https://edabit.com/challenge/covbapJ32obi9PuSy)
