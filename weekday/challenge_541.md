# Challenge 541 - Strictly Increasing or Decreasing

Write a function that takes a list and determines whether it's strictly increasing, strictly decreasing, or neither.

## Examples
```python
check([1, 2, 3]) ➞ "increasing"

check([3, 2, 1]) ➞ "decreasing"

check([1, 2, 1]) ➞ "neither"

check([1, 1, 2]) ➞ "neither"
```
## Notes

- The last example does NOT count as strictly increasing, since 1-indexed 1 is not strictly greater than the 0-indexed 1.
Input lists have a minimum length of 2.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def check(numbers: list[int]) -> str:
    return "" # Put your code here!!!


test(541, check)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                1,
                2,
                1
            ]
        ],
        "return": "neither"
    },
    {
        "args": [
            [
                9,
                7,
                1
            ]
        ],
        "return": "decreasing"
    },
    {
        "args": [
            [
                5,
                7
            ]
        ],
        "return": "increasing"
    },
    {
        "args": [
            [
                1,
                1,
                2
            ]
        ],
        "return": "neither"
    },
    {
        "args": [
            [
                1,
                3,
                5,
                7,
                9,
                10
            ]
        ],
        "return": "increasing"
    },
    {
        "args": [
            [
                5,
                6,
                5,
                7,
                9,
                10
            ]
        ],
        "return": "neither"
    },
    {
        "args": [
            [
                1,
                2,
                3
            ]
        ],
        "return": "increasing"
    },
    {
        "args": [
            [
                3,
                2,
                1
            ]
        ],
        "return": "decreasing"
    }
]
```
## Credits

Found on Edabit: [Strictly Increasing or Decreasing](https://edabit.com/challenge/hZi6AhWEzGASB7tWR)
