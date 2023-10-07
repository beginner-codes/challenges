# Challenge 767 - Generating Words from Names

Write a function that returns `True` if a given name can generate an array of words.

## Examples
```python
anagram("Justin Bieber", ["injures", "ebb", "it"]) ➞ True

anagram("Natalie Portman", ["ornamental", "pita"]) ➞ True

anagram("Chris Pratt", ["chirps", "rat"]) ➞ False
# Not all letters are used

anagram("Jeff Goldblum", ["jog", "meld", "bluffs"]) ➞ False
# "s" does not exist in the original name
```
## Notes

- Each letter in the name may only be used once.
- All letters in the name must be used.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. *
*[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a
key `args` that are a list of parameters your function should take. The `return` key is what your function should return
given the `args`.

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your
solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:

```python
from __future__ import annotations
from beginnercodes.challenges import test


def anagram(name: str, words: list[str]) -> bool:
    return False  # Put your code here!!!


test(767, anagram)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            "Matt Damon",
            [
                "madman"
            ]
        ],
        "return": false
    },
    {
        "args": [
            "Kristen Stewart",
            [
                "trinkets",
                "war",
                "set"
            ]
        ],
        "return": true
    },
    {
        "args": [
            "Graham Norton",
            [
                "graham",
                "not",
                "or"
            ]
        ],
        "return": false
    },
    {
        "args": [
            "Jeff Goldblum",
            [
                "jog",
                "meld",
                "bluffs"
            ]
        ],
        "return": false
    },
    {
        "args": [
            "Blake Shelton",
            [
                "betoken",
                "all",
                "she"
            ]
        ],
        "return": false
    }
]
```

## Credits

Found on Edabit: [Generating Words from Names](https://edabit.com/challenge/sDvjdcBrbHoXKvDsZ)
