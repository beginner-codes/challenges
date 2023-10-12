# Challenge 770 - Longest Word in a 7 Segment Display

Given a list of words, return the longest word which can fit on a 7 segment display.

Letters which do not fit on a 7 segment display are k, m, v, w and x. Do not count words which include these letters.

## Examples
```python
longest_7segment_word(["knighthood", "parental", "fridge", "clingfilm"]) ➞ "parental"

longest_7segment_word(["coding", "crackers", "edabit", "celebration"]) ➞ "celebration"

longest_7segment_word(["velocity", "mackerel", "woven", "kingsmen"]) ➞ ""
```
## Notes

- All words will be given in lowercase.
- Return an empty string if no words are eligible.
- If multiple valid words have the same length, return the first word that appears.

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


def longest_7segment_word(words: list[str]) -> str:
    return ""  # Put your code here!!!


test(770, longest_7segment_word)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                "knighthood",
                "parental",
                "fridge",
                "clingfilm"
            ]
        ],
        "return": "parental"
    },
    {
        "args": [
            [
                "front",
                "economist",
                "sector",
                "camp"
            ]
        ],
        "return": "sector"
    },
    {
        "args": [
            [
                "vain",
                "nature",
                "garlic",
                "garlic",
                "inspire",
                "thoughtful",
                "winner",
                "blade",
                "pillow",
                "fair",
                "goat",
                "bell",
                "lounge",
                "fair"
            ]
        ],
        "return": "thoughtful"
    },
    {
        "args": [
            [
                "winner",
                "twin",
                "establish"
            ]
        ],
        "return": "establish"
    },
    {
        "args": [
            [
                "maze",
                "human body",
                "move",
                "perceive",
                "maze",
                "scramble",
                "flavor",
                "delicate",
                "accessible"
            ]
        ],
        "return": "accessible"
    }
]
```

## Credits

Found on Edabit: [Longest Word in a 7 Segment Display](https://edabit.com/challenge/kAQT4vMX2iEAcs8uJ)
