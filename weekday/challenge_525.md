# Challenge 525 - Count the Towers 

Create a function that counts the number of towers.

## Examples
```python
count_towers([
  ["     ##         "],
  ["##   ##        ##"],
  ["##   ##   ##   ##"],
  ["##   ##   ##   ##"]
]) ➞ 4

count_towers([
  ["                         ##"],
  ["##             ##   ##   ##"],
  ["##        ##   ##   ##   ##"],
  ["##   ##   ##   ##   ##   ##"]
]) ➞ 6

count_towers([
  ["##"],
  ["##"]
]) ➞ 1
```
## Notes

- You are given a 2D matrix.
- Towers are two characters in length.
- Towers are made only of the character `#`.
- Some tests have no towers, return `0`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def count_towers(towers: list[list[str]]) -> int:
    return 0 # Put your code here!!!


test(525, count_towers)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                [
                    "                         ##"
                ],
                [
                    "##             ##   ##   ##"
                ],
                [
                    "##        ##   ##   ##   ##"
                ],
                [
                    "##   ##   ##   ##   ##   ##"
                ]
            ]
        ],
        "return": 6
    },
    {
        "args": [
            [
                [
                    ""
                ]
            ]
        ],
        "return": 0
    },
    {
        "args": [
            [
                [
                    "##"
                ],
                [
                    "##"
                ]
            ]
        ],
        "return": 1
    },
    {
        "args": [
            [
                [
                    "##   ##          "
                ],
                [
                    "##   ##          "
                ],
                [
                    "##   ##   ##   ##"
                ],
                [
                    "##   ##   ##   ##"
                ]
            ]
        ],
        "return": 4
    },
    {
        "args": [
            [
                [
                    "                                              "
                ],
                [
                    "##   ##   ##   ##   ##   ##   ##   ##   ##   ##"
                ],
                [
                    "##   ##   ##   ##   ##   ##   ##   ##   ##   ##"
                ],
                [
                    "##   ##   ##   ##   ##   ##   ##   ##   ##   ##"
                ]
            ]
        ],
        "return": 10
    }
]
```
## Credits

Found on Edabit: [Count the Towers](https://edabit.com/challenge/5q3FdCvrXtwQRoGmP)
