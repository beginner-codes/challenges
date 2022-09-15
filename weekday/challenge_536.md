# Challenge 536 - Split and Delimit

Write a function that splits a string into substrings of size n, adding a specified delimiter between each of the pieces.

## Examples
```python
split_and_delimit("bellow", 2, "&") ➞ "be&ll&ow"

split_and_delimit("magnify", 3, ":") ➞ "mag:nif:y"

split_and_delimit("poisonous", 2, "~") ➞ "po~is~on~ou~s"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def split_and_delimit(string: str, size: int, delimiter: str) -> str:
    return "" # Put your code here!!!


test(536, split_and_delimit)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "nebulous",
            1,
            "#"
        ],
        "return": "n#e#b#u#l#o#u#s"
    },
    {
        "args": [
            "magnify",
            3,
            ":"
        ],
        "return": "mag:nif:y"
    },
    {
        "args": [
            "shape-shifting",
            5,
            "^"
        ],
        "return": "shape^-shif^ting"
    },
    {
        "args": [
            "poisonous",
            2,
            "~"
        ],
        "return": "po~is~on~ou~s"
    },
    {
        "args": [
            "bellow",
            2,
            "&"
        ],
        "return": "be&ll&ow"
    }
]
```
## Credits

Found on Edabit: [Split and Delimit](https://edabit.com/challenge/LgXMXThsKcYtdYHrb)
