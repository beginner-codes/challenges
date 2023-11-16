# Challenge 793 - Word Riddles

What does the word LFAND represent? It represents the word Finland, because F is in LAND!

Create a function which replicates this to create brand-new original riddles! For the purposes of this challenge, take the string of letters before the word "in", and insert them after the letter following "in".

##  Examples
```python
make_word_riddle("Finland") ➞ "LFAND"

make_word_riddle("dinner") ➞ "NDER"

make_word_riddle("tkinter") ➞ "TTKER"

make_word_riddle("STRINGS") ➞ "GSTRS"
```
## Notes

- All words given will contain only one occurrence of "in" (so no occurrences of the words Insulin, Infinity, etc.)
- There will be no examples of Interest, Pin, or Ping, etc. as there is no clear way to insert the strings
- Return in all CAPS.

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


def make_word_riddle(word: str) -> str:
    return ""  # Put your code here!!!


test(793, make_word_riddle)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            "attainablities"
        ],
        "return": "AATTABLITIES"
    },
    {
        "args": [
            "administrations"
        ],
        "return": "IADMSTRATIONS"
    },
    {
        "args": [
            "choriocarcinoma"
        ],
        "return": "OCHORIOCARCMA"
    },
    {
        "args": [
            "metalinguistics"
        ],
        "return": "GMETALUISTICS"
    },
    {
        "args": [
            "STRINGS"
        ],
        "return": "GSTRS"
    }
]
```

## Credits

Found on Edabit: [Word Riddles](https://edabit.com/challenge/mwicBKcq3gTGhsGsW)
