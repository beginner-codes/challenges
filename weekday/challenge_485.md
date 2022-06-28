# Challenge 485 - Filter Words

Write a function that receives a list of words and a mask. Return a list of words, sorted alphabetically, that match the given mask.

The `*` is a wildcard and will match any character. Any other character in the mask must be an exact match. If there are more characters in the string than in the mask, it is not a match.

## Examples
```python
filter_words([”red”, “dee”, “cede”, “reed”, “creed”, “decree”], “*re**”) ➞ [“creed”]

filter_words([”red”, “dee”, “cede”, “reed”, “creed”, “decree”], “***”) ➞ [“dee”, “ree”]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def filter_words(words: list[str], mask: str) -> list[str]:
    return []  # Put your code here!!!


test(485, filter_words)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "cee",
                "dee",
                "eer",
                "erd",
                "ere",
                "red",
                "ree",
                "cede",
                "cere",
                "cree",
                "deer",
                "dere",
                "dree",
                "rede",
                "reed",
                "ceder",
                "cedre",
                "cered",
                "creed",
                "decree",
                "recede"
            ],
            "*re**"
        ],
        "return": [
            "creed"
        ]
    },
    {
        "args": [
            [
                "cee",
                "dee",
                "eer",
                "erd",
                "ere",
                "red",
                "ree",
                "cede",
                "cere",
                "cree",
                "deer",
                "dere",
                "dree",
                "rede",
                "reed",
                "ceder",
                "cedre",
                "cered",
                "creed",
                "decree",
                "recede"
            ],
            "***"
        ],
        "return": [
            "cee",
            "dee",
            "eer",
            "erd",
            "ere",
            "red",
            "ree"
        ]
    },
    {
        "args": [
            [
                "cee",
                "dee",
                "eer",
                "erd",
                "ere",
                "red",
                "ree",
                "cede",
                "cere",
                "cree",
                "deer",
                "dere",
                "dree",
                "rede",
                "reed",
                "ceder",
                "cedre",
                "cered",
                "creed",
                "decree",
                "recede"
            ],
            "******"
        ],
        "return": [
            "decree",
            "recede"
        ]
    },
    {
        "args": [
            [
                "cee",
                "dee",
                "eer",
                "erd",
                "ere",
                "red",
                "ree",
                "cede",
                "cere",
                "cree",
                "deer",
                "dere",
                "dree",
                "rede",
                "reed",
                "ceder",
                "cedre",
                "cered",
                "creed",
                "decree",
                "recede"
            ],
            "c*d**"
        ],
        "return": [
            "ceder",
            "cedre"
        ]
    },
    {
        "args": [
            [
                "cee",
                "dee",
                "eer",
                "erd",
                "ere",
                "red",
                "ree",
                "cede",
                "cere",
                "cree",
                "deer",
                "dere",
                "dree",
                "rede",
                "reed",
                "ceder",
                "cedre",
                "cered",
                "creed",
                "decree",
                "recede"
            ],
            "d***"
        ],
        "return": [
            "deer",
            "dere",
            "dree"
        ]
    },
    {
        "args": [
            [
                "cee",
                "dee",
                "eer",
                "erd",
                "ere",
                "red",
                "ree",
                "cede",
                "cere",
                "cree",
                "deer",
                "dere",
                "dree",
                "rede",
                "reed",
                "ceder",
                "cedre",
                "cered",
                "creed",
                "decree",
                "recede"
            ],
            "r***"
        ],
        "return": [
            "rede",
            "reed"
        ]
    }
]
```
## Credits

Found on Edabit: [Scrambled Letters](https://edabit.com/challenge/f48nSAebxBNMfmc9D)
