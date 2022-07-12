# Challenge 483 - Sharing is Caring

Given a list of numbers, create a function that removes 25% from every number in the list except the smallest number, and adds the total amount removed to the smallest number.

## Examples
```python
show_the_love([4, 1, 4]) ➞ [3, 3, 3]

show_the_love([16, 10, 8]) ➞ [12, 7.5, 14.5]

show_the_love([2, 100]) ➞ [27, 75]
```
## Notes

- There will only be one smallest number in a given list.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def show_the_love(numbers: list[int]) -> list[int | float]:
    return []  # Put your code here!!!


test(483, show_the_love)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                4,
                1,
                4
            ]
        ],
        "return": [
            3,
            3,
            3
        ]
    },
    {
        "args": [
            [
                16,
                10,
                8
            ]
        ],
        "return": [
            12,
            7.5,
            14.5
        ]
    },
    {
        "args": [
            [
                2,
                100
            ]
        ],
        "return": [
            27,
            75
        ]
    },
    {
        "args": [
            [
                75,
                64,
                55
            ]
        ],
        "return": [
            56.25,
            48.0,
            89.75
        ]
    },
    {
        "args": [
            [
                84,
                94,
                26,
                80,
                16
            ]
        ],
        "return": [
            63.0,
            70.5,
            19.5,
            60.0,
            87.0
        ]
    }
]
```
## Credits

Found on Edabit: [Sharing is Caring](https://edabit.com/challenge/pqpkRBP4YT5dwBDHm)
