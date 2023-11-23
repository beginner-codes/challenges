# Challenge 798 - Find the Largest Prime within a Range

Given two integers as arguments, create a function that finds the largest prime within the range of the two integers.

## Examples
```python
fat_prime(2, 10) ➞ 7
# range [2, 3, 4, 5, 6, 7, 8, 9, 10] and the largest prime is 7.

fat_prime(10, 2) ➞ 7
# [10, 9, 8, 7, 6, 5, 4, 3, 2] and the largest prime is 7.

fat_prime(4, 24) ➞ 23
# range [4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24] the largest prime is 23.
```
## Notes

- All numbers will be positive integers.

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


def fat_prime(a: int, b: int) -> int:
    return 0  # Put your code here!!!


test(798, fat_prime)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            4,
            24
        ],
        "return": 23
    },
    {
        "args": [
            10,
            2
        ],
        "return": 7
    },
    {
        "args": [
            200,
            100
        ],
        "return": 199
    },
    {
        "args": [
            2,
            10
        ],
        "return": 7
    },
    {
        "args": [
            7,
            49
        ],
        "return": 47
    }
]
```

## Credits

Found on Edabit: [Plant Trees 🌲](https://edabit.com/challenge/3gziWsCxqGwGGZmr5)
