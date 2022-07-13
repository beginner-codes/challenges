# Challenge 459 - Rotated Words

Some characters do not change after a rotation of 180 degrees. They can be read, although sometimes in a different way. For example, uppercase letters `"H"`, `"I"`, `"N"`, `"O"`, `"S"`, `"X"`, `"Z"` after rotation are not changed, the letter `"M"` becomes a `"W"`, and vice versa.

So, the word `"WOW"` turns into the word `"MOM"`. On the other hand, the word `"HOME"` cannot be rotated.

Find the number of unique readable Rotated Words in the input string txt (without duplicates).

## Examples
```python
rotated_words("HSSN") ➞ 1
# String can be rotated to a valid string

rotated_words("OS IS UPDATED") ➞ 2
# "OS" and "IS" can be rotated to a valid string
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from beginnercodes.challenges import test


def rotated_words(string: str) -> int:
    return 0  # Put your code here!!!


test(449, rotated_words)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "HSSN"
        ],
        "return": 1
    },
    {
        "args": [
            "ON"
        ],
        "return": 1
    },
    {
        "args": [
            "OS IS UPDATED"
        ],
        "return": 2
    },
    {
        "args": [
            "WHO IS WHO"
        ],
        "return": 2
    },
    {
        "args": [
            "JS"
        ],
        "return": 0
    }
]
```
## Credits

Found on Edabit: [Rotated Words](https://edabit.com/challenge/aEMgdg3zgznbnDMpz)
