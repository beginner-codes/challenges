# Challenge 645 - Two is the Difference

Create a function that takes an array of integers and returns all pairs of integers that have a difference of two. The resulting array should be sorted in ascending order of values.

## Examples
```python
difference_two([1, 2, 3, 4]) ➞ [[1, 3], [2, 4]]

difference_two([1, 23, 3, 4, 7]) ➞ [[1, 3]]

difference_two([4, 3, 1, 5, 6]) ➞ [[1, 3], [3, 5], [4, 6]]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def difference_two(numbers: list[int]) -> list[list[int]]:
    return []  # Put your code here!!!


test(645, difference_two)  # Tell it which challenge to test against
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
                4
            ]
        ],
        "return": [
            [
                1,
                3
            ],
            [
                2,
                4
            ]
        ]
    },
    {
        "args": [
            [
                1,
                23,
                3,
                4,
                7
            ]
        ],
        "return": [
            [
                1,
                3
            ]
        ]
    },
    {
        "args": [
            [
                4,
                3,
                1,
                5,
                6
            ]
        ],
        "return": [
            [
                1,
                3
            ],
            [
                3,
                5
            ],
            [
                4,
                6
            ]
        ]
    }
]
```
## Credits

Found on Edabit: [Two is the Difference](https://edabit.com/challenge/xzisrRDwWT8prHtiQ)
