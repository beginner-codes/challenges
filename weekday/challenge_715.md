# Challenge 715 - Number Pairs

Create a function that determines how many number pairs are embedded in a space-separated string.

## Examples
```python
number_pairs("1 2 1 2 1 3 2") ➞ 2
# (1, 1), (2, 2)

number_pairs("10 20 20 10 10 30 50 10 20") ➞ 3
# (10, 10), (20, 20), (10, 10)

number_pairs("2 3 4 1") ➞ 0
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def number_pairs(numbers: str) -> int:
    return 0  # Put your code here!!!


test(715, number_pairs)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "10 20 20 10 10 30 50 10 20 50 50 30 20"
        ],
        "return": 6
    },
    {
        "args": [
            "2 3 4 1"
        ],
        "return": 0
    },
    {
        "args": [
            "1 2 1 2 1 3 2"
        ],
        "return": 2
    },
    {
        "args": [
            "2 3 5 11 1 11 5 7 9 13 17 3 8 7 2 1"
        ],
        "return": 6
    },
    {
        "args": [
            "10 20 20 10 10 30 50 10 20"
        ],
        "return": 3
    }
]
```
## Credits

Found on Edabit: [Number Pairs](https://edabit.com/challenge/rMwssAueJjn9FmjZC)
