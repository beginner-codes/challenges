# Challenge 488 - Do All Bigrams Exist?

You are given an input array of bigrams, and an array of words.

Write a function that returns `True` if every single bigram from this array can be found at least once in an array of words.

## Examples
```python
can_find(["at", "be", "th", "au"], ["beautiful", "the", "hat"]) ➞ True

can_find(["ay", "be", "ta", "cu"], ["maybe", "beta", "abet", "course"]) ➞ False
# "cu" does not exist in any of the words.

can_find(["th", "fo", "ma", "or"], ["the", "many", "for", "forest"]) ➞ True

can_find(["oo", "mi", "ki", "la"], ["milk", "chocolate", "cooks"]) ➞ False
```
## Notes

- A bigram is string of two consecutive characters in the same word.
- If the list of words is empty, return `False`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

def can_find(bigrams: list[str], words: list[str]) -> bool:
    return False  # Put your code here!!!


test(488, can_find)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "at",
                "be",
                "th",
                "au"
            ],
            [
                "beautiful",
                "the",
                "hat"
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                "bo",
                "ta",
                "el",
                "st",
                "ca"
            ],
            [
                "books",
                "table",
                "cap",
                "hostel"
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                "la",
                "te"
            ],
            [
                "latte"
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                "th",
                "fo",
                "ma",
                "or"
            ],
            [
                "the",
                "many",
                "for",
                "forest"
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                "ay",
                "be",
                "ta",
                "cu"
            ],
            [
                "maybe",
                "beta",
                "abet",
                "course"
            ]
        ],
        "return": false
    }
]
```
## Credits

Found on Edabit: [Do All Bigrams Exist?](https://edabit.com/challenge/7QPHWACcDihT3AM6b)
