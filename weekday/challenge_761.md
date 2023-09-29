# Challenge 761 - Valid Hex Code

Create a function that determines whether a string is a valid hex code.

A hex code must begin with a octothorpe `#` and is exactly 6 characters in length. Each character must be a digit from 0-9 or an alphabetic character from A-F. All alphabetic characters may be uppercase or lowercase.

## Examples
```python
is_valid_hex_code("#CD5C5C") ➞ True

is_valid_hex_code("#EAECEE") ➞ True

is_valid_hex_code("#eaecee") ➞ True

is_valid_hex_code("#CD5C58C") ➞ False
# Length exceeds 6

is_valid_hex_code("#CD5C5Z") ➞ False
# Not all alphabetic characters in A-F

is_valid_hex_code("#CD5C&C") ➞ False
# Contains unacceptable character

is_valid_hex_code("CD5C5C") ➞ False
# Missing #
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. *
*[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a
key `args` that are a list of parameters your function should take. The `return` key is what your function should return
given the `args`.

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your
solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:

```python
from __future__ import annotations
from beginnercodes.challenges import test


def is_valid_hex_code(hex_code: str) -> bool:
    return False  # Put your code here!!!


test(761, is_valid_hex_code)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            "#ZCCZCC"
        ],
        "return": false
    },
    {
        "args": [
            "#123456"
        ],
        "return": true
    },
    {
        "args": [
            "#CD5C&C"
        ],
        "return": false
    },
    {
        "args": [
            "#123CCCD"
        ],
        "return": false
    },
    {
        "args": [
            "#987654"
        ],
        "return": true
    }
]
```

## Credits

Found on Edabit: [Valid Hex Code](https://edabit.com/challenge/9p5tMqyYENTmD9Nh5)
