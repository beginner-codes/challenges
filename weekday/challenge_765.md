# Challenge 765 - Check If the Brick Fits through the Hole

Write the function that takes three dimensions of a brick: height (a), width (b) and depth (c) and returns `True` if this brick can fit into a hole with the width (w) and height (h).

## Examples
```python
does_brick_fit(1, 1, 1, 1, 1) ➞ True

does_brick_fit(1, 2, 1, 1, 1) ➞ True

does_brick_fit(1, 2, 2, 1, 1) ➞ False
```
## Notes

- You can turn the brick with any side towards the hole.
- We assume that the brick fits if its sizes equal the ones of the hole (i.e. brick size should be less than or equal to the size of the hole, not strictly less).
- You can't put a brick in at a non-orthogonal angle.

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


def does_brick_fit(a: int, b: int, c: int, w: int, h: int) -> bool:
    return False  # Put your code here!!!


test(765, does_brick_fit)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            2,
            2,
            2,
            1,
            2
        ],
        "return": false
    },
    {
        "args": [
            1,
            1,
            1,
            1,
            1
        ],
        "return": true
    },
    {
        "args": [
            1,
            2,
            1,
            1,
            1
        ],
        "return": true
    },
    {
        "args": [
            1,
            2,
            2,
            1,
            1
        ],
        "return": false
    },
    {
        "args": [
            1,
            2,
            2,
            1,
            2
        ],
        "return": true
    },
    {
        "args": [
            1,
            2,
            2,
            2,
            1
        ],
        "return": true
    }
]
```

## Credits

Found on Edabit: [Check If the Brick Fits through the Hole](https://edabit.com/challenge/EyzmkffNRiEBtjAmf)
