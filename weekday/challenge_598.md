# Challenge 598 - Verbed Nouns

Create a function that ends the first word of a phrase with `"ed"`, essentially verbifying a noun.

## Examples
```python
verbify("cheese burger") ➞ "cheesed burger"

verbify("salt water") ➞ "salted water"

verbify("orange juice") ➞ "oranged juice"

verbify("shredded cheese") ➞ "shredded cheese"
```
## Notes

- Change only the first word.
- Note that some words may already end in `"e"` or `"ed"`.
- All phrases will be in lowercase.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def verbify(phrase: str) -> str:
    return ""  # Put your code here!!!


test(598, verbify)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "shredded cheese"
        ],
        "return": "shredded cheese"
    },
    {
        "args": [
            "air plane"
        ],
        "return": "aired plane"
    },
    {
        "args": [
            "cheese burger"
        ],
        "return": "cheesed burger"
    },
    {
        "args": [
            "bean toast"
        ],
        "return": "beaned toast"
    },
    {
        "args": [
            "pumpkin pie"
        ],
        "return": "pumpkined pie"
    }
]
```
## Credits

Found on Edabit: [Verbed Nouns](https://edabit.com/challenge/hPCtfpyXDDawsz6xw)
