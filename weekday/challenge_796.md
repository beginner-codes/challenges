# Challenge 796 - Simplifying to Simplest Ratio

Create a function which simplifies a given fraction into its simplest ratio. Return the fraction as a string.

## Examples
```python
simplify_frac("2/4") ➞ "1/2"

simplify_frac("15/25") ➞ "3/5"

simplify_frac("4/9") ➞ "4/9"
```
## Notes

- Fractions are given as strings
- Return the same fraction if it is already in its simplified ratio

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


def simplify_frac(fraction: str) -> str:
    return ""  # Put your code here!!!


test(796, simplify_frac)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            "20/80"
        ],
        "return": "1/4"
    },
    {
        "args": [
            "3/10"
        ],
        "return": "3/10"
    },
    {
        "args": [
            "12/13"
        ],
        "return": "12/13"
    },
    {
        "args": [
            "10/95"
        ],
        "return": "2/19"
    },
    {
        "args": [
            "8/41"
        ],
        "return": "8/41"
    }
]
```

## Credits

Found on Edabit: [Simplifying to Simplest Ratio](https://edabit.com/challenge/Qjn6B93kXLj2Kq5jB)
