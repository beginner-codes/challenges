# Challenge 735 - Numeric Seesaw

A number is left-heavy if the digits on the left side are larger than the digits on the right. It is right-heavy if the
digits on the right side are larger than the digits on the left. Else, it is balanced.

Create a function that takes in an integer and classifies it into one of the three mutually exclusive
categories: `left`, `right` or `balanced`. For inputs with an odd number of integers, ignore the middle number.

## Examples

```python
seesaw(3449) ➞ "right"
# since 34 < 49

seesaw(1143113) ➞ "left"
# since 114 > 113 (3 is the fulcrum)

seesaw(585585) ➞ "balanced"
# since 585 == 585
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


def seesaw(number: int) -> str:
    return ""  # Put your code here!!!


test(735, seesaw)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
  {
    "args": [
      111
    ],
    "return": "balanced"
  },
  {
    "args": [
      585585
    ],
    "return": "balanced"
  },
  {
    "args": [
      5855
    ],
    "return": "left"
  },
  {
    "args": [
      5558
    ],
    "return": "right"
  },
  {
    "args": [
      3449
    ],
    "return": "right"
  }
]
```

## Credits

Found on Edabit: [Numeric Seesaw](https://edabit.com/challenge/yGhSu82pSoGjZCRDy)
