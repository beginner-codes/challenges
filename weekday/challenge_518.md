# Challenge 518 - Reverse the String (with a catch)

Create a function that takes a string and returns the reversed string. However, there's a few rules to follow in order to make the challenge interesting:

- The UPPERCASE/lowercase positions must be kept in the same order as the original string (see example #1 and #2).
- Spaces must be kept in the same order as the original string (see example #3).

## Examples
```python
special_reverse_string("Beginner.Codes") ➞ "Sedoc.renNigeb"

special_reverse_string("UPPER lower") ➞ "REWOL reppu"

special_reverse_string("1 23 456") ➞ "6 54 321"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def special_reverse_string(string: str) -> str:
    return "" # Put your code here!!!


test(518, special_reverse_string)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "UPPER lower"
        ],
        "return": "REWOL reppu"
    },
    {
        "args": [
            "Beginner.Codes"
        ],
        "return": "Sedoc.renNigeb"
    },
    {
        "args": [
            "addition(3, 2) = 5"
        ],
        "return": "5=)2,3(noit id d a"
    },
    {
        "args": [
            "Hello World!"
        ],
        "return": "!dlro Wolleh"
    },
    {
        "args": [
            "It's known that CSS means Cascading Style Sheets"
        ],
        "return": "Stee hsely tsgn IDA csacs Naemsscta Htnwo Nks'ti"
    }
]
```
## Credits

Found on Edabit: [Reverse the String (with a catch)](https://edabit.com/challenge/hZ4HzhboCJ5dDiNve)
