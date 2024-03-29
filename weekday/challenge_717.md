# Challenge 717 - 3n + 1 Problem (Collatz Conjecture)

A Collatz sequence is generated by repeatedly applying the following rules to an integer and then to each resulting integer in turn:

- If even: divide by 2.
- If odd: multiply by 3, then add 1.

The Collatz algorithm has been tested and found to always reach 1 for all positive integers.

Create a function that, when given two positive integers, returns the string `"a"` if the first integer took fewer steps to reach 1 than the second when passed through the Collatz sequence, or `"b"` if the second integer took fewer steps to reach 1 than the first.

## Examples
```python
collatz(10, 15) ➞ "a"
# Because 10.0 - 5.0 - 16.0 - 8.0 - 4.0 - 2.0 - 1.0: 6 steps
# 15.0 - 46.0 - 23.0 - 70.0 - 35.0 - 106.0 - 53.0 - 160.0 - 80.0 - 40.0 - 20.0 - 10.0 - 5.0 - 16.0 - 8.0 - 4.0 - 2.0 - 1.0: 17 steps

collatz(13, 16) ➞ "b"

collatz(53782, 72534) ➞ "b"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def collatz(a: int, b: int) -> str:
    return ""  # Put your code here!!!


test(717, collatz)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            4,
            3
        ],
        "return": "a"
    },
    {
        "args": [
            13,
            16
        ],
        "return": "b"
    },
    {
        "args": [
            1723817263,
            837249873748
        ],
        "return": "a"
    },
    {
        "args": [
            556238,
            667822
        ],
        "return": "b"
    },
    {
        "args": [
            72221,
            11198
        ],
        "return": "b"
    }
]
```
## Credits

Found on Edabit: [3n + 1 Problem (Collatz Conjecture)](https://edabit.com/challenge/6JNHBeGxY8dhTaPhs)
