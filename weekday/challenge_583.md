# Challenge 583 - Convert to Hex

Create a function that takes a string's characters as ASCII and returns each character's hexadecimal value as a string.

## Examples
```python
convert_to_hex("hello world") ➞ "68 65 6c 6c 6f 20 77 6f 72 6c 64"

convert_to_hex("Big Boi") ➞ "42 69 67 20 42 6f 69"

convert_to_hex("Marty Poppinson") ➞ "4d 61 72 74 79 20 50 6f 70 70 69 6e 73 6f 6e"
```
## Notes

- Each byte must be seperated by a space.
- All alpha hex characters must be lowercase.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def convert_to_hex(string: str) -> str:
    return ""  # Put your code here!!!


test(583, convert_to_hex)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "oh dear"
        ],
        "return": "6f 68 20 64 65 61 72"
    },
    {
        "args": [
            "i hate C#"
        ],
        "return": "69 20 68 61 74 65 20 43 23"
    },
    {
        "args": [
            "i love C++ , not really"
        ],
        "return": "69 20 6c 6f 76 65 20 43 2b 2b 20 2c 20 6e 6f 74 20 72 65 61 6c 6c 79"
    },
    {
        "args": [
            "abcdefghi"
        ],
        "return": "61 62 63 64 65 66 67 68 69"
    },
    {
        "args": [
            "Big Boi"
        ],
        "return": "42 69 67 20 42 6f 69"
    }
]
```
## Credits

Found on Edabit: [Convert to Hex](https://edabit.com/challenge/g6yjSfTpDkX2STnSX)
