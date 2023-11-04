# Challenge 785 - Create a Stair

Write a function which takes an integer and returns a string representing an upward stair with the given number of steps. Each step will be represented by combinations of underscores, newlines, and vertical lines.

So, if you print the result for a stair with three steps, it will look something like this:
```
      _
    _|
  _|
_|
```
It's a crude and rickety stair, but challenging yourself in your favorite programming language is worth it.

## Examples
```python
stair(1)  ➞ "  _\n_|"
# 2 spaces, 1 underscore, 1 newline, 1 underscore, 1 vertical line

stair(2)  ➞ "    _\n  _|\n_|"
# 4 spaces, 1 undescore, 1 newline, 2 spaces, 1 underscore,
# 1 vertical line, 1 newline, 1 underscore, 1 vertical line

stair(3) ➞ "      _\n    _|\n  _|\n_|"
# 6 spaces, 1 undescore, 1 newline, 4 spaces, 1 underscore,
# 1 vertical line, 1 newline, 2 spaces, ...

stair(4) ➞ "        _\n      _|\n    _|\n  _|\n_|"
# 8 spaces, 1 undescore, 1 newline, 6 spaces, 1 underscore,
# 1 vertical line,  ...
```
## Notes

- All numbers are positive.
- For zero, return `"___"` (three underscores).

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


def stair(steps: int) -> str:
    return ""  # Put your code here!!!


test(785, stair)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            0
        ],
        "return": "___"
    },
    {
        "args": [
            2
        ],
        "return": "    _\n  _|\n_|"
    },
    {
        "args": [
            1
        ],
        "return": "  _\n_|"
    },
    {
        "args": [
            5
        ],
        "return": "          _\n        _|\n      _|\n    _|\n  _|\n_|"
    },
    {
        "args": [
            3
        ],
        "return": "      _\n    _|\n  _|\n_|"
    }
]
```

## Credits

Found on Edabit: [Create a Stair](https://edabit.com/challenge/ZF9e922XuRaMu43Wp)
