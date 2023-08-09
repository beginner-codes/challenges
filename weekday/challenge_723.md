# Challenge 723 - Cumulative List Sum

Create a function that takes a list of numbers and returns a list where each number is the sum of itself and all previous numbers in the list.

## Examples
```python
cumulative_sum([1, 2, 3]) ➞ [1, 3, 6]

cumulative_sum([1, -2, 3]) ➞ [1, -1, 2]

cumulative_sum([3, 3, -2, 408, 3, 3]) ➞ [3, 6, 4, 412, 415, 418]
```
## Notes

- Return an empty list if the input is an empty list.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def cumulative_sum(numbers: list[int]) -> list[int]:
    return []  # Put your code here!!!


test(723, cumulative_sum)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                1,
                -2,
                3
            ]
        ],
        "return": [
            1,
            -1,
            2
        ]
    },
    {
        "args": [
            [
                1,
                2,
                3
            ]
        ],
        "return": [
            1,
            3,
            6
        ]
    },
    {
        "args": [
            [
                -1,
                -2,
                -3
            ]
        ],
        "return": [
            -1,
            -3,
            -6
        ]
    },
    {
        "args": [
            []
        ],
        "return": []
    },
    {
        "args": [
            [
                3,
                3,
                -2,
                408,
                3,
                3,
                0,
                66,
                2,
                -2,
                2,
                3,
                4,
                2,
                -47,
                3,
                3,
                2
            ]
        ],
        "return": [
            3,
            6,
            4,
            412,
            415,
            418,
            418,
            484,
            486,
            484,
            486,
            489,
            493,
            495,
            448,
            451,
            454,
            456
        ]
    },
    {
        "args": [
            [
                1
            ]
        ],
        "return": [
            1
        ]
    }
]
```
## Credits

Found on Edabit: [Cumulative List Sum](https://edabit.com/challenge/qCLK8BomNpXTtFYTn)
