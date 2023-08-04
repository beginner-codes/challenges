# Challenge 720 - Change the Word

Given a string, reverse its order, change lowercase letters to uppercase and increment uppercase letters by one (e.g. A becomes B, C becomes D, Z becomes A).

## Examples
```python
change_string("ApPle") ➞ "ELQPB"

change_string("draGON") ➞ "OPHARD"

change_string("ZebrA") ➞ "BRBEA"
```
## Notes

- Remember capital `"Z"` becomes `"A"`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def change_string(string: str) -> string:
    return ""  # Put your code here!!!


test(720, change_string)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "draGON"
        ],
        "return": "OPHARD"
    },
    {
        "args": [
            "ZebrA"
        ],
        "return": "BRBEA"
    },
    {
        "args": [
            "ApPle"
        ],
        "return": "ELQPB"
    },
    {
        "args": [
            "MElon"
        ],
        "return": "NOLFN"
    },
    {
        "args": [
            "sNaKe"
        ],
        "return": "ELAOS"
    }
]
```
## Credits

Found on Edabit: [Change the Word](https://edabit.com/challenge/eKhy6Af4v3Yr8RfBE)
