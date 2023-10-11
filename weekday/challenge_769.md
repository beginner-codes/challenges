# Challenge 769 - Solve a Linear Equation

Create a function that returns the value of `x` (the "unknown" in the equation). Each equation will be formatted like this:
```
x + 6 = 12
```
## Examples
```python
solve("x + 43 = 50") ➞ 7

solve("x - 9 = 10") ➞ 19

solve("x + 300 = 100") ➞ -200
```
## Notes
- `x` will always be in the same place (you will not find an equation like `6 + x = 12`).
- Every equation will include either subtraction or addition.
- `x` may be negative.

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


def solve(equation: str) -> int:
    return 0  # Put your code here!!!


test(769, solve)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            "x + 43 = 50"
        ],
        "return": 7
    },
    {
        "args": [
            "x - 0 = 0"
        ],
        "return": 0
    },
    {
        "args": [
            "x + -500 = -200"
        ],
        "return": 300
    },
    {
        "args": [
            "x + 300 = 100"
        ],
        "return": -200
    },
    {
        "args": [
            "x + 188 = 866"
        ],
        "return": 678
    },
    {
        "args": [
            "x - 9 = 10"
        ],
        "return": 19
    }
]
```

## Credits

Found on Edabit: [Solve a Linear Equation](https://edabit.com/challenge/fpJXv7Qn9LCxX8FYq)
