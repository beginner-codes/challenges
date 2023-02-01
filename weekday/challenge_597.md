# Challenge 597 - Are Letters in the Second String Present in the First?

Create a function that accepts a list of two strings and checks if all letters in the second string are present in the first string.

## Examples
```python
letter_check(["trances", "nectar"]) ➞ True

letter_check(["compadres", "DRAPES"]) ➞ True

letter_check(["parses", "parsecs"]) ➞ False
```
## Notes

- Function should not be case-sensitive (as indicated in the second example).
- Both strings are presented as a single argument in the form of a list.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def letter_check(words: list[str]) -> bool:
    return False  # Put your code here!!!


test(597, letter_check)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "THE EYES",
                "they see"
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                "trances",
                "nectar"
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                "deltas",
                "slated"
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                "assert",
                "staring"
            ]
        ],
        "return": false
    },
    {
        "args": [
            [
                "arches",
                "later"
            ]
        ],
        "return": false
    }
]
```
## Credits

Found on Edabit: [Are Letters in the Second String Present in the First?](https://edabit.com/challenge/dFz2PDjQkXZ9FhEaz)
