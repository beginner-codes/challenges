# Challenge 529 - Longest Sequence of Consecutive Zeroes 

Write a function that returns the longest sequence of consecutive zeroes in a binary string.

## Examples
```python
longest_zero("01100001011000") ➞ "0000"

longest_zero("100100100") ➞ "00"

longest_zero("11111") ➞ ""
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def longest_zero(string: str) -> str:
    return "" # Put your code here!!!


test(529, longest_zero)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "1000000000011101"
        ],
        "return": "0000000000"
    },
    {
        "args": [
            "01100001011000"
        ],
        "return": "0000"
    },
    {
        "args": [
            "111111"
        ],
        "return": ""
    },
    {
        "args": [
            "101010101"
        ],
        "return": "0"
    },
    {
        "args": [
            "111101"
        ],
        "return": "0"
    }
]
```
## Credits

Found on Edabit: [Longest Sequence of Consecutive Zeroes](https://edabit.com/challenge/KbFxyTPiP4GMvxw68)
