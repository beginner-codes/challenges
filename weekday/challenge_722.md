# Challenge 722 - Snail Race

Steve and Maurice have racing snails. They each have three, one each slow, medium, and fast. Although Steve's snails are all a bit stronger than Maurice's, Maurice has a trick up his sleeve. His plan is:

- Round 1: Sacrifice his slowest snail against Steve's fastest.
- Round 2: Use his middle snail against Steve's slowest.
- Round 3: Use his fastest snail against Steve's middle.

Create a function that determines whether Maurice's plan will work by outputting `True` if Maurice wins 2/3 games.

The function inputs:

- A list of slow, medium, and fast snails for Maurice.
- A list of slow, medium, and fast snails for Steve.

## Examples
```python
maurice_wins([3, 5, 10], [4, 7, 11]) ➞ True
# Since the matches are (3, 11), (5, 4) and (10, 7), Maurice wins 2 out of 3.

maurice_wins([6, 8, 9], [7, 12, 14]) ➞ False
# Since the matches are (6, 14), (8, 7) and (9, 12), Steve wins 2 out of 3.

maurice_wins([1, 8, 20], [2, 9, 100]) ➞ True
```
## Notes

- Maurice wins if his competing snail's speed strictly exceeds Steve's snail's speed.
- Steve will always play in this order: fast, slow, medium.
- The order you'll get the snails is always in ascending order.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def maurice_wins(maurices_snails: list[int], steves_snails: list[int]) -> bool:
    return False  # Put your code here!!!


test(722, maurice_wins)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                3,
                8,
                13
            ],
            [
                5,
                11,
                15
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                1,
                8,
                20
            ],
            [
                2,
                9,
                100
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                3,
                5,
                10
            ],
            [
                4,
                7,
                11
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                1,
                2,
                3
            ],
            [
                2,
                3,
                4
            ]
        ],
        "return": false
    },
    {
        "args": [
            [
                6,
                8,
                9
            ],
            [
                7,
                12,
                14
            ]
        ],
        "return": false
    },
    {
        "args": [
            [
                2,
                4,
                10
            ],
            [
                3,
                9,
                11
            ]
        ],
        "return": true
    }
]
```
## Credits

Found on Edabit: [Snail Race](https://edabit.com/challenge/DGpxmRkADuZaWHJxZ)
