# Challenge 700 - Find the Missing Letter

Create a function that takes a list of increasing letters and return the missing letter.

## Examples
```python
missing_letter(["a", "b", "c", "e", "f", "g"]) ➞ "d"

missing_letter(["O", "Q", "R", "S"]) ➞ "P"

missing_letter(["t", "u", "v", "w", "x", "z"]) ➞ "y"

missing_letter(["m", "o"]) ➞ "n"
```
## Notes

- Tests will always have exactly one letter missing.
- The length of the test list will always be at least two.
- Tests will be in one particular case (upper or lower but never both).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def missing_letters(letters: list[str]) -> str:
    return ""  # Put your code here!!!


test(700, missing_letters)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "B",
                "D"
            ]
        ],
        "return": "C"
    },
    {
        "args": [
            [
                "q",
                "s",
                "t"
            ]
        ],
        "return": "r"
    },
    {
        "args": [
            [
                "O",
                "Q",
                "R",
                "S"
            ]
        ],
        "return": "P"
    },
    {
        "args": [
            [
                "t",
                "u",
                "w",
                "x"
            ]
        ],
        "return": "v"
    },
    {
        "args": [
            [
                "t",
                "u",
                "v",
                "w",
                "x",
                "z"
            ]
        ],
        "return": "y"
    }
]
```
## Credits

Found on Edabit: [Find the Missing Letter](https://edabit.com/challenge/CqNoAPcQrckobTacs)
