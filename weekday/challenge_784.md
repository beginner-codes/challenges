# Challenge 784 - Ones and Zeroes

Write a function that returns `True` if every consecutive sequence of ones is followed by a consecutive sequence of zeroes of the same length.

## Examples
```python
same_length("110011100010") ➞ True

same_length("101010110") ➞ False

same_length("111100001100") ➞ True

same_length("111") ➞ False
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


def same_length(sequence: str) -> bool:
    return False  # Put your code here!!!


test(784, same_length)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            "1001"
        ],
        "return": false
    },
    {
        "args": [
            "101001"
        ],
        "return": false
    },
    {
        "args": [
            "10101110001100"
        ],
        "return": true
    },
    {
        "args": [
            "10010"
        ],
        "return": false
    },
    {
        "args": [
            "10"
        ],
        "return": true
    }
]
```

## Credits

Found on Edabit: [Ones and Zeroes](https://edabit.com/challenge/TZXG9RfcZ7T3o43QF)
