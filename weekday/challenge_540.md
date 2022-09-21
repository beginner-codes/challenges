# Challenge 540 - Max Adjacent Product

Given a list of integers, find the pair of adjacent elements that have the largest product and return that product.

## Examples
```python
adjacent_product([3, 6, -2, -5, 7, 3] ) ➞ 21

adjacent_product([5, 6, -4, 2, 3, 2, -23]) ➞ 30

adjacent_product([0, -1, 1, 24, 1, -4, 8, 10]) ➞ 80
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def adjacent_product(numbers: list[int]) -> int:
    return 0 # Put your code here!!!


test(540, adjacent_product)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                -23,
                4,
                -3,
                8,
                -12
            ]
        ],
        "return": -12
    },
    {
        "args": [
            [
                3,
                6,
                -2,
                -5,
                7,
                3
            ]
        ],
        "return": 21
    },
    {
        "args": [
            [
                1,
                0,
                1,
                0,
                1000
            ]
        ],
        "return": 0
    },
    {
        "args": [
            [
                -1,
                -2
            ]
        ],
        "return": 2
    },
    {
        "args": [
            [
                0,
                -1,
                1,
                24,
                1,
                -4,
                8,
                10
            ]
        ],
        "return": 80
    },
    {
        "args": [
            [
                5,
                6,
                -4,
                2,
                3,
                2,
                -23
            ]
        ],
        "return": 30
    }
]
```
## Credits

Found on Edabit: [Max Adjacent Product](https://edabit.com/challenge/DJa7PoKDhTTmwnxJg)
