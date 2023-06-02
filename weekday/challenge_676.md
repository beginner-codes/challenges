# Challenge 676 - Who is Currently Winning

You are given a list of scores. The even-indexed numbers are your scores at each turn. The odd-indexed numbers are your opponent's scores.

Create a function that turns this list of scores into a list of who is currently winning.

To illustrate (You - Y, Opponent - O):

Scores: `[5, 15, 17, 35, 16, 40, 66, 12, 10, 9]`

Y scores: `[5, 17, 16, 66, 10]`
O scores: `[15, 35, 40, 12, 9]`

Y cumulative scores: [5, 22, 38, 104, 114]
O cumulative scores: `[15, 50, 90, 102, 111]`

Who is currently winning: `["O", "O", "O", "Y", "Y"]`
## Examples
```python
currently_winning([10, 10, 22, 30, 5, 40]) ➞ ["T", "O", "O"]

currently_winning([5, 1, 2, 10]) ➞ ["Y", "O"]

currently_winning([10, 10, 5, 5, 2, 2, 1, 3, 100, 5]) ➞ ["T", "T", "T", "O", "Y"]
```
## Notes

- Write `"T"` if there is a tie at that point in the game.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def currently_winning(scores: list[int]) -> list[str]:
    return []  # Put your code here!!!


test(676, currently_winning)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                33,
                22,
                4,
                9,
                12,
                15,
                32,
                7,
                9,
                10,
                70,
                100
            ]
        ],
        "return": [
            "Y",
            "Y",
            "Y",
            "Y",
            "Y",
            "O"
        ]
    },
    {
        "args": [
            [
                5,
                15,
                17,
                35,
                16,
                40,
                66,
                12,
                10,
                9
            ]
        ],
        "return": [
            "O",
            "O",
            "O",
            "Y",
            "Y"
        ]
    },
    {
        "args": [
            [
                10,
                10,
                22,
                30,
                5,
                40
            ]
        ],
        "return": [
            "T",
            "O",
            "O"
        ]
    },
    {
        "args": [
            [
                10,
                10,
                5,
                5,
                2,
                2,
                1,
                3,
                100,
                5
            ]
        ],
        "return": [
            "T",
            "T",
            "T",
            "O",
            "Y"
        ]
    },
    {
        "args": [
            [
                5,
                1,
                2,
                10
            ]
        ],
        "return": [
            "Y",
            "O"
        ]
    }
]
```
## Credits

Found on Edabit: [Who is Currently Winning](https://edabit.com/challenge/epMcaSNzBFSF5uB89)
