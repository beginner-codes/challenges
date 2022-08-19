# Challenge 522 - Order by Length First 

Graded lexicographic order (grlex order for short) is a way of ordering words that:

- First orders words by length.
- Then orders words of the same size by their dictionary order.
- For example, in grlex order:
```
"tray" < "trapped" since "tray" has length 4 while "trapped" has length 7.
"trap" < "tray" since both have length 4, but "trap" comes before "tray" in the dictionary.
```
Given a list of words, return that list in grlex order.

## Examples
```python
make_grlex(["small", "big"]) ➞ ["big", "small"]

make_grlex(["cat", "ran", "for", "the", "rat"]) ➞ ["cat", "for", "ran", "rat", "the"]

make_grlex(["this", "is", "a", "small", "test"]) ➞ ["a", "is", "test", "this", "small"]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def make_grlex(words: list[str]) -> list[str]:
    return [] # Put your code here!!!


test(522, make_grlex)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "small",
                "big"
            ]
        ],
        "return": [
            "big",
            "small"
        ]
    },
    {
        "args": [
            [
                "big",
                "cat",
                "ran",
                "for",
                "the",
                "fat",
                "rat"
            ]
        ],
        "return": [
            "big",
            "cat",
            "fat",
            "for",
            "ran",
            "rat",
            "the"
        ]
    },
    {
        "args": [
            [
                "this",
                "is",
                "a",
                "small",
                "test"
            ]
        ],
        "return": [
            "a",
            "is",
            "test",
            "this",
            "small"
        ]
    },
    {
        "args": [
            [
                "let",
                "us",
                "try",
                "some",
                "long",
                "test",
                "to",
                "see",
                "if",
                "this",
                "works",
                "as",
                "it",
                "should"
            ]
        ],
        "return": [
            "as",
            "if",
            "it",
            "to",
            "us",
            "let",
            "see",
            "try",
            "long",
            "some",
            "test",
            "this",
            "works",
            "should"
        ]
    }
]
```
## Credits

Found on Edabit: [Order by Length First](https://edabit.com/challenge/qLMZ2hEvrhRSSSnQw)
