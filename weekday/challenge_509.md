# Challenge 509 - Numbered Alphabet

Create a function that converts a string of letters to their respective number in the alphabet.

## Examples
```python
alph_num("XYZ") ➞ "23 24 25"

alph_num("ABCDEF") ➞ "0 1 2 3 4 5"

alph_num("JAVASCRIPT") ➞ "9 0 21 0 18 2 17 8 15 19"
```
## Notes

- Make sure the numbers are spaced.
- All letters will be UPPERCASE.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def alph_num(string: str) -> str:
    return ""  # Put your code here!!!


test(509, alph_num)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "ABCD"
        ],
        "return": "0 1 2 3"
    },
    {
        "args": [
            "BCDA"
        ],
        "return": "1 2 3 0"
    },
    {
        "args": [
            "AAA"
        ],
        "return": "0 0 0"
    },
    {
        "args": [
            "XYZ"
        ],
        "return": "23 24 25"
    }
]
```
## Credits

Found on Edabit: [Numbered Alphabet](https://edabit.com/challenge/e6fL5EiwGZcsW7C5D)
