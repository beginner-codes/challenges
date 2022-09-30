# Challenge 545 - Balancing Scales

Given a list with an odd number of elements, return whether the scale will tip `"left"` or `"right"` based on the sum of the numbers. The scale will tip on the direction of the largest total. If both sides are equal, return `"balanced"`.

## Examples
```python
scale_tip([0, 0, "I", 1, 1]) ➞ "right"
# 0 < 2 so it will tip right

scale_tip([1, 2, 3, "I", 4, 0, 0]) ➞ "left"
# 6 > 4 so it will tip left

scale_tip([5, 5, 5, 0, "I", 10, 2, 2, 1]) ➞ "balanced"
# 15 = 15 so it will stay balanced
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def scale_tip(scale: list[int|str]) -> str:
    return "" # Put your code here!!!


test(545, scale_tip)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                500,
                0,
                0,
                "I",
                500,
                0,
                0
            ]
        ],
        "return": "balanced"
    },
    {
        "args": [
            [
                500,
                0,
                0,
                "I",
                32,
                53,
                12
            ]
        ],
        "return": "left"
    },
    {
        "args": [
            [
                1,
                300,
                "I",
                300,
                2
            ]
        ],
        "return": "right"
    },
    {
        "args": [
            [
                500,
                0,
                0,
                "I",
                302,
                53,
                12
            ]
        ],
        "return": "left"
    },
    {
        "args": [
            [
                0,
                0,
                0,
                "I",
                1,
                1,
                1
            ]
        ],
        "return": "right"
    }
]
```
## Credits

Found on Edabit: [Balancing Scales](https://edabit.com/challenge/xPmfKHShmuKL5Qf9u)
