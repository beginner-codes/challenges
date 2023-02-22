# Challenge 610 - What's the Missing Letter?

Given a string of letters in the English alphabet, return the letter that's missing from the string. The missing letter will make the string be in alphabetical order (from A to Z).

If there are no missing letters in the string, return `"No Missing Letter"`.

## Examples
```python
missing_letter("abdefg") ➞ "c"

missing_letter("mnopqs") ➞ "r"

missing_letter("tuvxyz") ➞ "w"

missing_letter("ghijklmno") ➞ "No Missing Letter"
```
## Notes

- The given string will never have more than one missing letter.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def missing_letter(letters: str) -> str:
    return ""  # Put your code here!!!


test(610, missing_letter)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "jlm"
        ],
        "return": "k"
    },
    {
        "args": [
            "abdefg"
        ],
        "return": "c"
    },
    {
        "args": [
            "tuvxyz"
        ],
        "return": "w"
    },
    {
        "args": [
            "qrtuv"
        ],
        "return": "s"
    },
    {
        "args": [
            "ghijklmno"
        ],
        "return": "No Missing Letter"
    }
]
```
## Credits

Found on Edabit: [EarlyWhat's the Missing Letter? Birds](https://edabit.com/challenge/Q5bu2bXxXxfWtvmjy)
