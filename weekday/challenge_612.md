# Challenge 612 - Convert to Ordinal


Create a function that takes an integer and returns it as an ordinal number. An Ordinal Number is a number that tells the position of something in a list, such as 1st, 2nd, 3rd, 4th, 5th, etc.

## Examples
```python
convert_to_ordinal(553) ➞ "553-RD"

convert_to_ordinal(34) ➞ "34-TH"

convert_to_ordinal(1231) ➞ "1231-ST"

convert_to_ordinal(22) ➞ "22-ND"

convert_to_ordinal(412) ➞ "412-TH"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def convert_to_ordinal(number: int) -> str:
    return ""  # Put your code here!!!


test(612, convert_to_ordinal)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            12341
        ],
        "return": "12341-ST"
    },
    {
        "args": [
            3222
        ],
        "return": "3222-ND"
    },
    {
        "args": [
            711
        ],
        "return": "711-TH"
    },
    {
        "args": [
            412
        ],
        "return": "412-TH"
    },
    {
        "args": [
            1
        ],
        "return": "1-ST"
    },
    {
        "args": [
            563
        ],
        "return": "563-RD"
    },
    {
        "args": [
            334
        ],
        "return": "334-TH"
    },
    {
        "args": [
            213
        ],
        "return": "213-TH"
    }
]
```
## Credits

Found on Edabit: [Return the End Letters of Numbers](https://edabit.com/challenge/GYJcHcgbpKYE75vYd)
