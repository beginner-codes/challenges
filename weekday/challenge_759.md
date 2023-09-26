# Challenge 759 - Sum of Negative Integers

Create a function that takes a string containing integers as well as other characters and return the sum of the negative integers only.

## Examples
```python
negative_sum("-12 13%14&-11") ➞ -23
# -12 + -11 = -23

negative_sum("22 13%14&-11-22 13 12") ➞ -33
# -11 + -22 = -33
```
## Notes

- There is at least one negative integer.

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


def negative_sum(string: str) -> int:
    return 0  # Put your code here!!!


test(759, negative_sum)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            "-12 13%14&-2 0 12 -4"
        ],
        "return": -18
    },
    {
        "args": [
            "-12 -8"
        ],
        "return": -20
    },
    {
        "args": [
            "-12 13%14&-11"
        ],
        "return": -23
    },
    {
        "args": [
            "33%14&-1 12 a 21 -2 b c"
        ],
        "return": -3
    },
    {
        "args": [
            "22 13%14&-11-22 13 12"
        ],
        "return": -33
    }
]
```

## Credits

Found on Edabit: [Sum of Negative Integers](https://edabit.com/challenge/q3zrcjja7uWHejxf6)
