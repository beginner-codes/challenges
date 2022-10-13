# Challenge 553 - Word Builder

In this challenge, you have to build a word from the scrambled letters contained in the first given list. For establishing how to assign the spots to the letters, you will use the positions contained in the second given list.
```python
letters = ["e", "t", "s", "t"]
positions = [1, 3, 2, 0]

Step 1 ➞ Letter "e" goes to index 1 ➞ _  e  _   _
Step 2 ➞ Letter "t" goes to index 3 ➞ _  e  _   t
Step 3 ➞ Letter "s" goes to index 2 ➞ _  e  s   t
Step 4 ➞ Letter "t" goes to index 0 ➞ t  e  s   t
```
Given the two lists letters (containing the scrambled letters of the word) and positions (containing the indexes of the letters), implement a function that returns the resulting word as a string.

## Examples
```python
word_builder(["e", "t", "s", "t"], [1, 3, 2, 0]) ➞ "test"

word_builder(["g", "e", "o"], [1, 0, 2]) ➞ "ego"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def word_builder(letters: list[str], positions: list[int]) -> str:
    return "" # Put your code here!!!


test(553, word_builder)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "s",
                "o",
                "r",
                "t",
                "e",
                "d"
            ],
            [
                0,
                1,
                2,
                3,
                4,
                5
            ]
        ],
        "return": "sorted"
    },
    {
        "args": [
            [
                "e",
                "t",
                "s",
                "t"
            ],
            [
                1,
                3,
                2,
                0
            ]
        ],
        "return": "test"
    },
    {
        "args": [
            [
                "l",
                "e",
                "h",
                "n",
                "l",
                "c",
                "a",
                "e",
                "g"
            ],
            [
                3,
                5,
                1,
                6,
                4,
                0,
                2,
                8,
                7
            ]
        ],
        "return": "challenge"
    },
    {
        "args": [
            [
                "e",
                "i",
                "l",
                "g",
                "x",
                "h",
                "p",
                "o",
                "c",
                "r",
                "i",
                "a",
                "c"
            ],
            [
                1,
                3,
                0,
                6,
                2,
                10,
                9,
                5,
                4,
                7,
                11,
                8,
                12
            ]
        ],
        "return": "lexicographic"
    },
    {
        "args": [
            [
                "g",
                "e",
                "o"
            ],
            [
                1,
                0,
                2
            ]
        ],
        "return": "ego"
    }
]
```
## Credits

Found on Edabit: [Word Builder](https://edabit.com/challenge/dYHH7CmYeWGXdEhCx)
