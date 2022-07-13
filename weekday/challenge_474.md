# Challenge 474 - Keeping Count

Given a number, create a function that returns a new number using these rules:

- For each digit, replace it by the number of times it appears in the number.
- The final instance of the number will be an integer, not a string.

## Worked Example
```python
digit_count(136116) ➞ 312332
# The number 1 appears thrice, so replace all 1s with 3s.
# The number 3 appears only once, so replace all 3s with 1s.
# The number 6 appears twice, so replace all 6s with 2s.
# Return as an integer.
```
## Examples
```python
digit_count(221333) ➞ 221333

digit_count(136116) ➞ 312332

digit_count(2) ➞ 1
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def digit_count(number: int) -> int:
    return 0  # Put your code here!!!


test(474, digit_count)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            221333
        ],
        "return": 221333
    },
    {
        "args": [
            136116
        ],
        "return": 312332
    },
    {
        "args": [
            2
        ],
        "return": 1
    },
    {
        "args": [
            3410515780
        ],
        "return": 1122222112
    },
    {
        "args": [
            24677734541
        ],
        "return": 13133313131
    },
    {
        "args": [
            79825929634
        ],
        "return": 13121323111
    },
    {
        "args": [
            36123594675
        ],
        "return": 22112211212
    },
    {
        "args": [
            62849835970
        ],
        "return": 11212211211
    }
]
```
## Credits

Found on Edabit: [Keeping Count](https://edabit.com/challenge/frRRffQGSrPTknfxY)
