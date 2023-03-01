# Challenge 615 - Temperature Converter

Create a function that converts Celsius to Fahrenheit and vice versa.

- C to F: `temp * 9 / 5 + 32`
- F to C: `(temp - 32) * 5 / 9`

## Examples
```python
convert("35*C") ➞ "95*F"

convert("19*F") ➞ "-7*C"

convert("33") ➞ "Error"
```
## Notes

- Round to the nearest integer.
- If the input is incorrect, return `"Error"`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def convert(temp: str) -> str:
    return ""  # Put your code here!!!


test(615, convert)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "85*C"
        ],
        "return": "185*F"
    },
    {
        "args": [
            "18*C"
        ],
        "return": "64*F"
    },
    {
        "args": [
            "-90*C"
        ],
        "return": "-130*F"
    },
    {
        "args": [
            "19*F"
        ],
        "return": "-7*C"
    },
    {
        "args": [
            "0*F"
        ],
        "return": "-18*C"
    }
]
```
## Credits

Found on Edabit: [Temperature Converter](https://edabit.com/challenge/pSrCZFim6Y8HcS9Yc)
