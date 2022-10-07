# Challenge 550 - Remove The Word!

Create a function that takes a list and a string. The function should remove the letters in the string from the list, and return the remaining letters as a list.

## Examples
```python
remove_letters(["s", "t", "r", "i", "n", "g", "w"], "string") ➞ ["w"]

remove_letters(["b", "b", "l", "l", "g", "n", "o", "a", "w"], "balloon") ➞ ["b", "g", "w"]

remove_letters(["d", "b", "t", "e", "a", "i"], "edabit") ➞ []
```
## Notes

- If number of times a letter appears in the list is greater than the number of times the letter appears in the string, the extra letters should be left behind (see example #2).
- If all the letters in the list are used in the string, the function should return an empty list (see example #3).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def remove_letters(letters: list[str], word: str) -> list[str]:
    return [] # Put your code here!!!


test(550, remove_letters)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "e",
                "e",
                "e",
                "g",
                "d",
                ".",
                "i",
                "o",
                "n",
                "c",
                "r",
                "b",
                "s",
                "n"
            ],
            "beginner.codes"
        ],
        "return": []
    },
    {
        "args": [
            [
                "b",
                "b",
                "l",
                "l",
                "g",
                "n",
                "o",
                "a",
                "w"
            ],
            "balloon"
        ],
        "return": [
            "b",
            "g",
            "w"
        ]
    },
    {
        "args": [
            [
                "t",
                "t",
                "e",
                "s",
                "t",
                "u"
            ],
            "testing"
        ],
        "return": [
            "t",
            "u"
        ]
    },
    {
        "args": [
            [
                "s",
                "t",
                "r",
                "i",
                "n",
                "g",
                "w"
            ],
            "string"
        ],
        "return": [
            "w"
        ]
    }
]
```
## Credits

Found on Edabit: [Remove The Word!](https://edabit.com/challenge/gH3QMvF3czMDjENkk)
