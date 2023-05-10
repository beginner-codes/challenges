# Challenge 660 - Gold Distribution

You and a friend have found some piles of gold. You have decided to follow some simple rules to distribute the gold between you..

- Choose the bigger gold pile, either from the far left or far right.
- If the weight of both piles is equal, choose the left pile.

Create a function that takes an array of gold piles and returns a two-element array with `[Your Gold, Your Friend's Gold]`. You will go first.

## Examples
```python
gold_distribution([4, 2, 9, 5, 2, 7]) ➞ [14, 15]
# You will choose 7, Remaining piles = [4, 2, 9, 5, 2]
# Your friend will choose 4, Remaining piles = [2, 9, 5, 2]
# You will choose 2, Remaining piles = [9, 5, 2]
# Your friend will choose 9, Remaining piles = [5, 2]
# You will choose 5, Remaining piles = [2]
# Your friend will choose 2
# You = 7+2+5 = 14, Your Friend = 4+9+2 = 15

gold_distribution([10, 1000, 2, 1]) ➞ [12, 1001]

gold_distribution([10, 9, 1, 2, 8, 4]) ➞ [16, 18]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def gold_distribution(gold_piles: list[int], win: int) -> list[int]:
    return []  # Put your code here!!!


test(660, gold_distribution)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                4,
                7,
                2,
                9,
                5,
                2
            ]
        ],
        "return": [
            11,
            18
        ]
    },
    {
        "args": [
            [
                9,
                32,
                12,
                43,
                1,
                55
            ]
        ],
        "return": [
            130,
            22
        ]
    },
    {
        "args": [
            [
                10,
                9,
                1,
                2,
                8,
                4
            ]
        ],
        "return": [
            16,
            18
        ]
    },
    {
        "args": [
            [
                19,
                22,
                1,
                5,
                7,
                31
            ]
        ],
        "return": [
            58,
            27
        ]
    },
    {
        "args": [
            [
                2,
                2,
                2,
                2,
                2,
                2
            ]
        ],
        "return": [
            6,
            6
        ]
    }
]
```
## Credits

Found on Edabit: [Gold Distribution](https://edabit.com/challenge/bJxNHk7aovkx8Q776)
