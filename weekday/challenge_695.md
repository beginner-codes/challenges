# Challenge 695 - Shared vs. Unique Letters

Create a function that takes in two words as input and returns a list of three elements, in the following order:

- Shared letters between two words.
- Letters unique to word 1.
- Letters unique to word 2.

Each element should have unique letters, and have each letter be alphabetically sorted.

## Examples
```python
letters("sharp", "soap") ➞ ["aps", "hr", "o"]

letters("board", "bored") ➞ ["bdor", "a", "e"]

letters("happiness", "envelope") ➞ ["enp", "ahis", "lov"]

letters("kerfuffle", "fluffy") ➞ ["flu", "ekr", "y"]
# Even with multiple matching letters (e.g. 3 f's), there should 
# only exist a single "f" in your first element.

letters("match", "ham") ➞ ["ahm", "ct", ""]
# "ham" does not contain any letters that are not found already 
# in "match".
```
## Notes

- Both words will be in lower case.
- You do not have to worry about punctuation, all words only have letters from [a-z].
- If an element contains no letters, return an empty string.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def letters(word_1: str, word_2: str) -> list[str]:
    return []  # Put your code here!!!


test(695, letters)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "happiness",
            "envelope"
        ],
        "return": [
            "enp",
            "ahis",
            "lov"
        ]
    },
    {
        "args": [
            "kerfuffle",
            "fluffy"
        ],
        "return": [
            "flu",
            "ekr",
            "y"
        ]
    },
    {
        "args": [
            "match",
            "ham"
        ],
        "return": [
            "ahm",
            "ct",
            ""
        ]
    },
    {
        "args": [
            "sharp",
            "soap"
        ],
        "return": [
            "aps",
            "hr",
            "o"
        ]
    },
    {
        "args": [
            "board",
            "bored"
        ],
        "return": [
            "bdor",
            "a",
            "e"
        ]
    }
]
```
## Credits

Found on Edabit: [Shared vs. Unique Letters](https://edabit.com/challenge/GaJkMnuHLuPmXZK7h)
