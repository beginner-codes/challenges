# Challenge 665 - A Simple Pair

Given an array of integers and an integer, find a pair of numbers from the array where their product is the integer.

If the pair is not found, return `None`/`Null`/etc..

## Examples
```python
simple_pair([1, 2, 3], 3) ➞ [1, 3]

simple_pair([1, 2, 3], 6) ➞ [2, 3]

simple_pair([1, 2, 3], 9) ➞ None
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def simple_pair(numbers: list[int], number: int) -> list[int] | None:
    return None  # Put your code here!!!


test(665, simple_pair)  # Tell it which challenge to test against
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
                6
            ],
            6
        ],
        "return": [
            1,
            6
        ]
    },
    {
        "args": [
            [
                0,
                0,
                2
            ],
            4
        ],
        "return": null
    },
    {
        "args": [
            [
                1,
                2,
                3
            ],
            7
        ],
        "return": null
    },
    {
        "args": [
            [
                -3,
                -2,
                -2,
                -1,
                0,
                1,
                2,
                3,
                4
            ],
            0
        ],
        "return": [
            -3,
            0
        ]
    },
    {
        "args": [
            [
                0,
                0,
                2,
                2
            ],
            4
        ],
        "return": [
            2,
            2
        ]
    }
]
```
## Credits

Found on Edabit: [A Simple Pair](https://edabit.com/challenge/PGqy3SRaobbtFfspW)
