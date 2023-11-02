# Challenge 783 - Ones, Threes and Nines

Given an integer determine how many nines, threes, and ones that number factors into. Output the result as a string following this format:
```python
"nines:your answer, threes:your answer, ones:your answer"
```

## Examples
```python
ones_threes_nines(10) ➞ "nines:1, threes:0, ones:1"

ones_threes_nines(15) ➞ "nines:1, threes:2, ones:0"

ones_threes_nines(22) ➞ "nines:2, threes:1, ones:1"
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


def ones_threes_nines(number: int) -> str:
    return ""  # Put your code here!!!


test(783, ones_threes_nines)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            22
        ],
        "return": "nines:2, threes:1, ones:1"
    },
    {
        "args": [
            15
        ],
        "return": "nines:1, threes:2, ones:0"
    },
    {
        "args": [
            10
        ],
        "return": "nines:1, threes:0, ones:1"
    },
    {
        "args": [
            1
        ],
        "return": "nines:0, threes:0, ones:1"
    },
    {
        "args": [
            25
        ],
        "return": "nines:2, threes:2, ones:1"
    }
]
```

## Credits

Found on Edabit: [Ones, Threes and Nines (Version #2)](https://edabit.com/challenge/8Fwv2f8My4kcNjMZh)
