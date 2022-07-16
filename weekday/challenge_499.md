# Challenge 499 - Word Overlapping

Given two words, overlap them in such a way, morphing the last few letters of the first word with the first few letters of the second word. Return the shortest overlapped word possible.

## Examples
```python
overlap("sweden", "denmark") ➞ "swedenmark"

overlap("honey", "milk") ➞ "honeymilk"

overlap("dodge", "dodge") ➞ "dodge"
```
## Notes

- All words will be given in lowercase.
- If no overlap is possible, return both words one after the other.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def overlap(word_a: str, word_b: str) -> str:
    return ""  # Put your code here!!!


test(498, overlap)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "sweden",
            "denmark"
        ],
        "return": "swedenmark"
    },
    {
        "args": [
            "honey",
            "milk"
        ],
        "return": "honeymilk"
    },
    {
        "args": [
            "dodge",
            "dodge"
        ],
        "return": "dodge"
    },
    {
        "args": [
            "colossal",
            "alligator"
        ],
        "return": "colossalligator"
    },
    {
        "args": [
            "leave",
            "eavesdrop"
        ],
        "return": "leavesdrop"
    },
    {
        "args": [
            "joshua",
            "osha"
        ],
        "return": "joshuaosha"
    },
    {
        "args": [
            "diction",
            "dictionary"
        ],
        "return": "dictionary"
    },
    {
        "args": [
            "massive",
            "mass"
        ],
        "return": "massivemass"
    }
]

```
## Credits

Found on Edabit: [Word Overlapping](https://edabit.com/challenge/gQgFJiNy8ZDCqaZb4)
