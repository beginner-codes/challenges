# Challenge 502 - Global Variable???

Create a function that returns how often it has been called previously (i.e. return the count value pre-increment).

## Examples
```python
counter() ➞ 0

counter() ➞ 1

counter() ➞ 2

counter() ➞ 3
```
## Bonus Challenge

Can you do this without a global?

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def counter() -> int:
    return 0  # Put your code here!!!


test(502, counter)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [],
        "return": 0
    },
    {
        "args": [],
        "return": 1
    },
    {
        "args": [],
        "return": 2
    },
    {
        "args": [],
        "return": 3
    },
    {
        "args": [],
        "return": 4
    },
    {
        "args": [],
        "return": 5
    },
    {
        "args": [],
        "return": 6
    },
    {
        "args": [],
        "return": 7
    },
    {
        "args": [],
        "return": 8
    },
    {
        "args": [],
        "return": 9
    },
    {
        "args": [],
        "return": 10
    },
    {
        "args": [],
        "return": 11
    }
]
```
## Credits

Found on Edabit: [Global Variable](https://edabit.com/challenge/C85NXJxetcYoF5eoy)
