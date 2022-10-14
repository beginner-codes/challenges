# Challenge 554 - Scoring a Field Goal

In (American) Football, a team can score if they manage to kick a ball through the goal (i.e. above the crossbar and between the uprights).

Create a function that returns `True` if the ball goes through the goal. You will be given a list of lists.

## Examples
```python
is_goal_scored([
  ["  #     #  "],
  ["  #  0  #  "],
  ["  #     #  "],
  ["  #######  "],
  ["     #     "],
  ["     #     "],
  ["     #     "]
]) ➞ True

is_goal_scored([
  ["  #0    #  "],
  ["  #     #  "],
  ["  #     #  "],
  ["  #######  "],
  ["     #     "],
  ["     #     "],
  ["     #     "]
]) ➞ True

is_goal_scored([
  ["  #     #  "],
  ["  #     #  "],
  ["  #     # 0"],
  ["  #######  "],
  ["     #     "],
  ["     #     "],
  ["     #     "]
]) ➞ False
```
## Notes

- All goals will be of the same size.
- All lists will be of equal length (11).
- A team can never score if it hits the crossbar or goes underneath it.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def is_goal_scored(kick: list[list[str]]) -> bool:
    return False # Put your code here!!!


test(554, is_goal_scored)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                [
                    "  #     #  "
                ],
                [
                    "  #     #  "
                ],
                [
                    "  #     #  "
                ],
                [
                    "  #######  "
                ],
                [
                    "     #    0"
                ],
                [
                    "     #     "
                ],
                [
                    "     #     "
                ]
            ]
        ],
        "return": false
    },
    {
        "args": [
            [
                [
                    "0 #     #  "
                ],
                [
                    "  #     #  "
                ],
                [
                    "  #     #  "
                ],
                [
                    "  #######  "
                ],
                [
                    "     #     "
                ],
                [
                    "     #     "
                ],
                [
                    "     #     "
                ]
            ]
        ],
        "return": false
    },
    {
        "args": [
            [
                [
                    "  #     #  "
                ],
                [
                    "  #     #  "
                ],
                [
                    "  #     # "
                ],
                [
                    "  #######  "
                ],
                [
                    "     #     "
                ],
                [
                    " 0   #     "
                ],
                [
                    "     #     "
                ]
            ]
        ],
        "return": false
    }
]
```
## Credits

Found on Edabit: [Scoring a Field Goal](https://edabit.com/challenge/AWYR47h7vCCwDmoXF)
