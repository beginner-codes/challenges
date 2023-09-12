# Challenge 748 - Unlucky Years

Create a function which returns how many Friday 13ths there are in a given year.

## Examples
```python
how_unlucky(2020) ➞ 2

how_unlucky(2026) ➞ 3

how_unlucky(2016) ➞ 1
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


def how_unlucky(year: int) -> int:
    return 0  # Put your code here!!!


test(748, how_unlucky)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            2002
        ],
        "return": 2
    },
    {
        "args": [
            2012
        ],
        "return": 3
    },
    {
        "args": [
            2039
        ],
        "return": 1
    },
    {
        "args": [
            2022
        ],
        "return": 1
    },
    {
        "args": [
            2042
        ],
        "return": 1
    }
]
```

## Credits

Found on Edabit: [Unlucky Years](https://edabit.com/challenge/MSX7AHcNiCZpCsiXY)
