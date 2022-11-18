# Challenge 575 - Anti-Divisors of a Number

The anti-divisors are numbers that do not divide a given number by the largest possible margin, and they can be found following a simple set of rules:

- Every number greater than `1` and lower than `n` is checked.
- Every checked number must not be a divisor of `n`.
- If the checked number is odd and it is a divisor of `n * 2 - 1` or `n * 2 + 1` it's an anti-divisor.
- If the checked number is even and it is a divisor of `n * 2`, it's an anti-divisor.

Given an integer `n`, implement a function that returns a list containing the anti-divisors of `n` sorted in ascending order.

## Examples
```python
anti_divisors(10) ➞ [3, 4, 7]
# 3 is a divisor of 21 (10 * 2 + 1)
# 4 is a divisor of 20 (10 * 2)
# 7 is a divisor of 21

anti_divisors(12) ➞ [5, 8]
# 5 is a divisor of 25 (12 * 2 + 1)
# 8 is a divisor of 24 (12 * 2)

anti_divisors(20) ➞ [3, 8, 13]
# 3 is a divisor of 39 (20 * 2 - 1)
# 8 is a divisor of 40 (20 * 2)
# 13 is a divisor of 39
```
## Notes

- The given `n` can be any integer, either positive, negative or `0`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def anti_divisors(n: int) -> list[int]:
    return []  # Put your code here!!!


test(575, anti_divisors)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            55
        ],
        "return": [
            2,
            3,
            10,
            22,
            37
        ]
    },
    {
        "args": [
            31
        ],
        "return": [
            2,
            3,
            7,
            9,
            21
        ]
    },
    {
        "args": [
            12
        ],
        "return": [
            5,
            8
        ]
    },
    {
        "args": [
            1
        ],
        "return": []
    },
    {
        "args": [
            0
        ],
        "return": []
    }
]
```
## Credits

Found on Edabit: [Anti-Divisors of a Number](https://edabit.com/challenge/GGAKNYFg2JEwxzcqk)
