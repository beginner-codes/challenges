# Challenge 477 - Sort By Index of Character

Write a function that sorts a list of characters alphabetically in ascending order (`a-z`) by the character at the n-th index.

## Examples
```python
sort_by_character(["az16", "by35", "cx24"], 2) ➞ ["cx24", "by35", "az16"]
# By 2nd character: ["x", "y", "z"] is in alphabetical order.

sort_by_character(["mayor", "apple", "petal"], 5) ➞ ["apple", "petal", "mayor"]
# By 5th character: ["e", "l", "r"] is in alphabetical order

sort_by_character(["mate", "team", "bade"], 3) ➞ ["team", "bade", "mate"]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def sort_by_character(words: list[str], index: int) -> list[str]:
    return []  # Put your code here!!!


test(477, sort_by_character)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "az16",
                "by35",
                "cx24"
            ],
            1
        ],
        "return": [
            "az16",
            "by35",
            "cx24"
        ]
    },
    {
        "args": [
            [
                "az16",
                "by35",
                "cx24"
            ],
            2
        ],
        "return": [
            "cx24",
            "by35",
            "az16"
        ]
    },
    {
        "args": [
            [
                "az16",
                "by35",
                "cx24"
            ],
            3
        ],
        "return": [
            "az16",
            "cx24",
            "by35"
        ]
    },
    {
        "args": [
            [
                "az16",
                "by35",
                "cx24"
            ],
            4
        ],
        "return": [
            "cx24",
            "by35",
            "az16"
        ]
    },
    {
        "args": [
            [
                "apple",
                "mayor",
                "bendy",
                "petal"
            ],
            5
        ],
        "return": [
            "apple",
            "petal",
            "mayor",
            "bendy"
        ]
    },
    {
        "args": [
            [
                "team",
                "mate",
                "bade"
            ],
            3
        ],
        "return": [
            "team",
            "bade",
            "mate"
        ]
    }
]
```
## Credits

Found on Edabit: [Sort By Index of Character](https://edabit.com/challenge/NQToxLLFCjugHWBoZ)
