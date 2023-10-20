# Challenge 776 - The Nearest Element

Given a list of integers, implement a function that returns the index of the number nearest to a given value. If two numbers are found to be equally distant from the value, the function returns the greatest of the two.

## Examples
```python
nearest_element(10, [1, 100, 1000]) ➞ 0
# 1 is the number nearest to 10.

nearest_element(50, [100, 49, 51]) ➞ 2
# 49 and 51 are equally distant from 50, with 51 being the greatest.

nearest_element(-20, [-50, -10, -30]) ➞ 1
# -10 and -30 are equally distant from -20, with -10 being the greatest.
```
## Notes

- Integers in the list are always unique. 

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


def nearest_element(value: int, numbers: list[int]) -> int:
    return 0  # Put your code here!!!


test(776, nearest_element)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            -50,
            [
                13,
                86,
                -49,
                -51,
                8,
                0
            ]
        ],
        "return": 2
    },
    {
        "args": [
            50,
            [
                100,
                49,
                51
            ]
        ],
        "return": 2
    },
    {
        "args": [
            10,
            [
                1,
                100,
                1000
            ]
        ],
        "return": 0
    },
    {
        "args": [
            100,
            [
                80,
                60,
                40
            ]
        ],
        "return": 0
    },
    {
        "args": [
            1,
            [
                0,
                -2,
                3,
                2,
                -1
            ]
        ],
        "return": 3
    }
]
```

## Credits

Found on Edabit: [The Nearest Element](https://edabit.com/challenge/tX5ZhY5EkduHAPZBh)
