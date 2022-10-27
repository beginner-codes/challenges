# Challenge 562 - Map the Letters in a String

Given a word, create a mapping that stores the indexes of each letter in a list.

- Make sure the letters are the keys.
- Make sure the indexes are stored as the values in a list.

## Examples
```python
map_letters("dodo") ➞ { "d": [0, 2], "o": [1, 3] }

map_letters("froggy") ➞ { "f":  [0], "r": [1], "o": [2], "g": [3, 4], "y": [5] }

map_letters("grapes") ➞ { "g": [0], "r": [1], "a": [2], "p": [3], "e": [4], "s": [5] }
```
## Notes

- All strings given will be lowercase.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def map_letters(word: str) -> dict[str, list[int]]:
    return {} # Put your code here!!!


test(562, map_letters)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "a"
        ],
        "return": {
            "a": [
                0
            ]
        }
    },
    {
        "args": [
            "aaaaaaabaaabaaabbb"
        ],
        "return": {
            "a": [
                0,
                1,
                2,
                3,
                4,
                5,
                6,
                8,
                9,
                10,
                12,
                13,
                14
            ],
            "b": [
                7,
                11,
                15,
                16,
                17
            ]
        }
    },
    {
        "args": [
            "imagining"
        ],
        "return": {
            "i": [
                0,
                4,
                6
            ],
            "m": [
                1
            ],
            "a": [
                2
            ],
            "g": [
                3,
                8
            ],
            "n": [
                5,
                7
            ]
        }
    },
    {
        "args": [
            "mummy"
        ],
        "return": {
            "m": [
                0,
                2,
                3
            ],
            "u": [
                1
            ],
            "y": [
                4
            ]
        }
    }
]
```
## Credits

Found on Edabit: [Map the Letters in a String](https://edabit.com/challenge/9CdF5hA7jRARpBwcF)
