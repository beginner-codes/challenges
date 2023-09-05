# Challenge 743 - Return the Most Frequent Character

Write a function that returns the most frequent character in a list of words.

## Examples
```python
most_frequent_char(["apple", "bandage", "yodel", "make"])
➞ ["a", "e"]

most_frequent_char(["music", "madness", "maniac", "motion"])
➞ ["m"]

most_frequent_char(["the", "hills", "are", "alive", "with", "the", "sound", "of", "music"])
➞ ["e", "h", "i"]
```
## Notes

- If multiple characters tie for most frequent, list all of them in alphabetical order.
- Words will be in lower case.

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


def most_frequent_char(words: list[str]) -> list[str]:
    return []  # Put your code here!!!


test(743, most_frequent_char)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                "music",
                "madness",
                "maniac",
                "motion"
            ]
        ],
        "return": [
            "m"
        ]
    },
    {
        "args": [
            [
                "apple",
                "bandage",
                "yodel",
                "make"
            ]
        ],
        "return": [
            "a",
            "e"
        ]
    },
    {
        "args": [
            [
                "the",
                "hills",
                "are",
                "alive",
                "with",
                "the",
                "sound",
                "of",
                "music"
            ]
        ],
        "return": [
            "e",
            "h",
            "i"
        ]
    },
    {
        "args": [
            [
                "let",
                "them",
                "eat",
                "cake"
            ]
        ],
        "return": [
            "e"
        ]
    },
    {
        "args": [
            [
                "potion",
                "master",
                "professor",
                "snape"
            ]
        ],
        "return": [
            "o",
            "s"
        ]
    }
]
```

## Credits

Found on Edabit: [Return the Most Frequent Character](https://edabit.com/challenge/KcD3bABvuryCfZAYv)
