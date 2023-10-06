# Challenge 766 - Number of Two or More Consecutive Ones

Create a function that counts the number of blocks of two or more adjacent 1s in a list.

## Examples
```python
count_ones([1, 0, 0, 1, 1, 0, 1, 1, 1]) ➞ 2
# Two instances: [1, 1] (middle) and [1, 1, 1] (end)

count_ones([1, 0, 1, 0, 1, 0, 1, 0]) ➞ 0

count_ones([1, 1, 1, 1, 0, 0, 0, 0]) ➞ 1

count_ones([0, 0, 0]) ➞ 0
```
## Notes

- A single 1 by itself (surrounded by a zero on its left and right), does not count towards the total.
- Each input will contain only zeroes and ones.

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


def count_ones(numbs: list[int]) -> int:
    return 0  # Put your code here!!!


test(766, count_ones)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                1,
                0,
                1,
                0,
                1,
                0,
                1,
                0
            ]
        ],
        "return": 0
    },
    {
        "args": [
            [
                1,
                1,
                1,
                1,
                0
            ]
        ],
        "return": 1
    },
    {
        "args": [
            [
                1,
                1,
                1,
                1,
                0,
                0,
                0,
                0
            ]
        ],
        "return": 1
    },
    {
        "args": [
            [
                1,
                0,
                0,
                0,
                1,
                0,
                0,
                1,
                1
            ]
        ],
        "return": 1
    },
    {
        "args": [
            [
                1,
                1,
                0,
                1,
                1,
                0,
                0,
                1,
                1
            ]
        ],
        "return": 3
    }
]
```

## Credits

Found on Edabit: [Number of Two or More Consecutive Ones](https://edabit.com/challenge/u4rHyBDs5RM2PfNxy)
