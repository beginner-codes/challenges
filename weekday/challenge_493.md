# Challenge 493 - Remix the String

Create a function that takes both a string and a list of integers and rearrange the letters in the string to be in the order specified by the index numbers. Return the "remixed" string.

## Examples
```python
remix("abcd", [0, 3, 1, 2]) ➞ "acdb"
The string you'll be returning will have:

# "a" at index 0
# "b" at index 3
# "c" at index 1
# "d" at index 2
# ... because the order of those characters maps to their corresponding numbers in the index list.

remix("PlOt", [1, 3, 0, 2]) ➞ "OPtl"

remix("computer", [0, 2, 1, 5, 3, 6, 7, 4]) ➞ "cmourpte"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def remix(string: str, indexes: list[str]) -> str:
    return ""  # Put your code here!!!


test(493, remix)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "abcd",
            [
                0,
                3,
                1,
                2
            ]
        ],
        "return": "acdb"
    },
    {
        "args": [
            "PlOt",
            [
                1,
                3,
                0,
                2
            ]
        ],
        "return": "OPtl"
    },
    {
        "args": [
            "computer",
            [
                0,
                2,
                1,
                5,
                3,
                6,
                7,
                4
            ]
        ],
        "return": "cmourpte"
    },
    {
        "args": [
            "twist",
            [
                4,
                0,
                1,
                2,
                3
            ]
        ],
        "return": "wistt"
    },
    {
        "args": [
            "responsibility",
            [
                0,
                6,
                8,
                11,
                10,
                7,
                13,
                5,
                3,
                2,
                4,
                12,
                1,
                9
            ]
        ],
        "return": "rtibliensyopis"
    },
    {
        "args": [
            "Interference",
            [
                6,
                9,
                10,
                11,
                7,
                3,
                0,
                2,
                5,
                1,
                8,
                4
            ]
        ],
        "return": "enrfeeIrcnte"
    },
    {
        "args": [
            "sequence",
            [
                5,
                7,
                3,
                4,
                0,
                1,
                2,
                6
            ]
        ],
        "return": "encqusee"
    }
]
```
## Credits

Found on Edabit: [Remix the String](https://edabit.com/challenge/EPXH424t2SSjMzms5)
