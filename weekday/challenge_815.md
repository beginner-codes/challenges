# Challenge 815 - Least Common Multiple

Create a function that takes two numbers as arguments and return the LCM (least common multiple) of the two numbers.

## Examples
```python
lcm(3, 5) ➞ 15

lcm(14, 28) ➞ 28

lcm(4, 6) ➞ 12
```
## Notes

- You may want to use the GCD to make this easier

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


def lcm(a: int, b: int) -> int:
    return 0  # Put your code here!!!


test(815, lcm)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            10000,
            333
        ],
        "return": 3330000
    },
    {
        "args": [
            6,
            10
        ],
        "return": 30
    },
    {
        "args": [
            30,
            60
        ],
        "return": 60
    },
    {
        "args": [
            102,
            2
        ],
        "return": 102
    },
    {
        "args": [
            75,
            135
        ],
        "return": 675
    }
]
```

## Credits

Found on Edabit: [GCD and LCM (Part 2)](https://edabit.com/challenge/a7WiKcyrTtggTym3f)
