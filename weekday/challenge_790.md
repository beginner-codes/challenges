# Challenge 790 - Happy Number

A happy number is a number which yields a 1 by repeatedly summing up the square of its digits. If such a process results in an endless cycle of numbers containing 4, the number is said to be an unhappy number.

Create a function that accepts a number and determines whether the number is a happy number or not. Return `True` if so, `False` otherwise.

## Examples
```python
is_happy(67) ➞ False

is_happy(89) ➞ False

is_happy(139) ➞ True

is_happy(1327) ➞ False

is_happy(2871) ➞ False

is_happy(3970) ➞ True
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


def is_happy(number: int) -> bool:
    return False  # Put your code here!!!


test(790, is_happy)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            10
        ],
        "return": true
    },
    {
        "args": [
            6329
        ],
        "return": true
    },
    {
        "args": [
            67
        ],
        "return": false
    },
    {
        "args": [
            10000
        ],
        "return": true
    },
    {
        "args": [
            1327
        ],
        "return": false
    }
]
```

## Credits

Found on Edabit: [Happy Number](https://edabit.com/challenge/rGAcibgZ6u9MtasfW)
