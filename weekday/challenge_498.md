# Challenge 498 - Triple Letter Groupings

Given a string, return a sorted list of words formed from the first three letters, then the next three letters, shifting by only one.

## Worked Example
```python
three_letter_collection("click") ➞ ["cli", "ick", "lic"]
# 1st word: "cli"
# 2nd word: "lic"
# 3rd word: "ick"
# Remember to sort the list!
```
## Examples
```python
three_letter_collection("slap") ➞ ["lap", "sla"]

three_letter_collection("cat") ➞ ["cat"]

three_letter_collection("hi") ➞ []
```
## Notes

- Return an empty list if given a word with less than 3 letters.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def three_letter_collection(word: str) -> list[str]:
    return []  # Put your code here!!!


test(4978, three_letter_collection)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "slap"
        ],
        "return": [
            "lap",
            "sla"
        ]
    },
    {
        "args": [
            "click"
        ],
        "return": [
            "cli",
            "ick",
            "lic"
        ]
    },
    {
        "args": [
            "cat"
        ],
        "return": [
            "cat"
        ]
    },
    {
        "args": [
            "hi"
        ],
        "return": []
    },
    {
        "args": [
            "e"
        ],
        "return": []
    },
    {
        "args": [
            ""
        ],
        "return": []
    },
    {
        "args": [
            "programming"
        ],
        "return": [
            "amm",
            "gra",
            "ing",
            "min",
            "mmi",
            "ogr",
            "pro",
            "ram",
            "rog"
        ]
    },
    {
        "args": [
            "antidisestablishmentarianism"
        ],
        "return": [
            "abl",
            "ani",
            "ant",
            "ari",
            "bli",
            "dis",
            "ent",
            "est",
            "hme",
            "ian",
            "idi",
            "ise",
            "ish",
            "ism",
            "lis",
            "men",
            "nis",
            "nta",
            "nti",
            "ria",
            "ses",
            "shm",
            "sta",
            "tab",
            "tar",
            "tid"
        ]
    },
    {
        "args": [
            "zoology"
        ],
        "return": [
            "log",
            "ogy",
            "olo",
            "ool",
            "zoo"
        ]
    },
    {
        "args": [
            "assassination"
        ],
        "return": [
            "ass",
            "ass",
            "ati",
            "ina",
            "ion",
            "nat",
            "sas",
            "sin",
            "ssa",
            "ssi",
            "tio"
        ]
    },
    {
        "args": [
            "bookkeeper"
        ],
        "return": [
            "boo",
            "eep",
            "epe",
            "kee",
            "kke",
            "okk",
            "ook",
            "per"
        ]
    }
]
```
## Credits

Found on Edabit: [Triple Letter Groupings](https://edabit.com/challenge/NybeH5L7wFPYeynCn)
