# Challenge 508 - Hold Your Breath!

You will be given a list of numbers which represent your character's altitude above sea level at regular intervals:

- Positive numbers represent height above the water.
- 0 is sea level.
- Negative numbers represent depth below the water's surface.

Create a function which returns whether your character survives their unsupervised diving experience, given a list of integers.

Your character starts with a breath meter of `10`, which is the maximum. When diving underwater, your breath meter decreases by `2` per item in the array. Watch out! If your breath diminishes to `0`, your character dies!

To prevent this, you can replenish your breath by `4` (up to the maximum of `10`) for each item in the array where you are at or above sea level.

Your function should return `True` if your character survives, and `False` if not.

## Worked Example
```python
diving_minigame([-5, -15, -4, 0, 5]) ➞ True

# Breath meter starts at 10.
# -5 is below water, so breath meter decreases to 8.
# -15 is below water, so breath meter decreases to 6.
# -4 is below water, so breath meter decreases to 4.
# 0 is at sea level, so breath meter increases to 8.
# 5 is above sea level and breath meter is capped at 10 (would've been 12 otherwise).
# Character survives!
```
## Examples
```python
diving_minigame([1, 2, 3, 4, 5, 6, 7, 8, 9, 10]) ➞ True

diving_minigame([-3, -6, -2, -6, -2]) ➞ False

diving_minigame([2, 1, 2, 1, -3, -4, -5, -3, -4]) ➞ False
```
## Notes

- Lists may be of any length.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def diving_minigame(altitudes: list[int]) -> bool:
    return False  # Put your code here!!!


test(508, diving_minigame)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                1,
                2,
                3,
                4,
                5,
                6,
                7,
                8,
                9,
                10
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                -5,
                -15,
                -4,
                0,
                5
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                0,
                -4,
                0,
                -4,
                -5,
                -2
            ]
        ],
        "return": true
    }
]
```
## Credits

Found on Edabit: [Hold Your Breath!](https://edabit.com/challenge/ZsLDkJfLGFkmjS2jE)
