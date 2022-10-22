# Challenge 559 - Land Perimeter

The function is given a map with `1` representing land, `0` representing water. A land cell can have four neighbors along its edges. Compute the total perimeter of shore-lines that are defined by land cells touching water or the outer edges of the map. Each cell edge has a length equal to `1`. An isolated cell without neighbors has a total perimeter length of `4`.

## Examples
```python
islands_perimeter([
  [0, 1, 0, 0],
  [1, 1, 1, 0],
  [0, 1, 0, 0],
  [1, 1, 0, 0]
]) ➞ 16

islands_perimeter([
  [1, 1, 1, 1, 1, 1],
  [1, 0, 0, 0, 0, 1],
  [1, 0, 1, 1, 0, 1],
  [1, 0, 0, 0, 0, 1],
  [1, 1, 1, 1, 1, 1],
]), 42)

islands_perimeter([
  [1, 0]
]) ➞ 4
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def islands_perimeter(islands: list[list[int]]) -> int:
    return 0 # Put your code here!!!


test(559, islands_perimeter)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                [
                    1,
                    1,
                    1,
                    1,
                    1,
                    1
                ],
                [
                    1,
                    0,
                    0,
                    0,
                    0,
                    1
                ],
                [
                    1,
                    0,
                    1,
                    1,
                    0,
                    1
                ],
                [
                    1,
                    0,
                    0,
                    0,
                    0,
                    1
                ],
                [
                    1,
                    1,
                    1,
                    1,
                    1,
                    1
                ]
            ]
        ],
        "return": 42
    },
    {
        "args": [
            [
                [
                    0,
                    0,
                    0,
                    0,
                    1,
                    1,
                    1,
                    1,
                    1,
                    1
                ],
                [
                    1,
                    1,
                    1,
                    1,
                    1,
                    1,
                    0,
                    0,
                    0,
                    0
                ]
            ]
        ],
        "return": 24
    },
    {
        "args": [
            [
                [
                    0,
                    1,
                    0,
                    0,
                    0,
                    0,
                    1,
                    1,
                    0,
                    1,
                    0,
                    0,
                    0,
                    0,
                    1,
                    0,
                    1,
                    1
                ],
                [
                    1,
                    1,
                    1,
                    0,
                    1,
                    0,
                    1,
                    1,
                    0,
                    1,
                    0,
                    1,
                    0,
                    0,
                    1,
                    0,
                    1,
                    1
                ],
                [
                    0,
                    1,
                    1,
                    0,
                    1,
                    0,
                    1,
                    1,
                    0,
                    1,
                    0,
                    1,
                    0,
                    0,
                    1,
                    0,
                    1,
                    0
                ],
                [
                    0,
                    1,
                    0,
                    0,
                    0,
                    0,
                    1,
                    1,
                    1,
                    1,
                    0,
                    1,
                    0,
                    0,
                    1,
                    0,
                    1,
                    0
                ],
                [
                    0,
                    1,
                    0,
                    1,
                    0,
                    0,
                    0,
                    0,
                    0,
                    0,
                    0,
                    1,
                    0,
                    1,
                    1,
                    1,
                    1,
                    1
                ],
                [
                    0,
                    0,
                    0,
                    1,
                    1,
                    1,
                    0,
                    1,
                    1,
                    1,
                    0,
                    1,
                    0,
                    0,
                    0,
                    1,
                    0,
                    0
                ],
                [
                    1,
                    1,
                    1,
                    1,
                    1,
                    1,
                    0,
                    1,
                    1,
                    1,
                    0,
                    1,
                    0,
                    1,
                    0,
                    1,
                    0,
                    1
                ],
                [
                    0,
                    0,
                    1,
                    0,
                    0,
                    1,
                    0,
                    1,
                    0,
                    0,
                    0,
                    0,
                    0,
                    1,
                    1,
                    1,
                    1,
                    1
                ]
            ]
        ],
        "return": 140
    },
    {
        "args": [
            [
                [
                    0,
                    0,
                    1,
                    1,
                    0,
                    0
                ],
                [
                    0,
                    0,
                    0,
                    0,
                    0,
                    1
                ],
                [
                    1,
                    0,
                    1,
                    1,
                    1,
                    1
                ],
                [
                    1,
                    0,
                    1,
                    1,
                    0,
                    1
                ],
                [
                    1,
                    1,
                    1,
                    1,
                    1,
                    1
                ]
            ]
        ],
        "return": 34
    },
    {
        "args": [
            [
                [
                    1,
                    0
                ]
            ]
        ],
        "return": 4
    },
    {
        "args": [
            [
                [
                    0,
                    1,
                    0,
                    0
                ],
                [
                    1,
                    1,
                    1,
                    0
                ],
                [
                    0,
                    1,
                    0,
                    0
                ],
                [
                    1,
                    1,
                    0,
                    0
                ]
            ]
        ],
        "return": 16
    }
]
```
## Credits

Found on Edabit: [Land Perimeter](https://edabit.com/challenge/kD2CfnakBqfNpBHnX)
