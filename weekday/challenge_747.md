# Challenge 747 - Longest Consecutive Run

A consecutive-run is a list of adjacent, consecutive integers. This list can be either increasing or decreasing. Create a function that takes a list of numbers and returns the length of the longest consecutive-run.

To illustrate:
```python
longestRun([1, 2, 3, 5, 6, 7, 8, 9]) ➞ 5
# Two consecutive runs: [1, 2, 3] and [5, 6, 7, 8, 9] (longest).
```
## Examples
```python
longest_run([1, 2, 3, 10, 11, 15]) ➞ 3
# Longest consecutive-run: [1, 2, 3].

longest_run([5, 4, 2, 1]) ➞ 2
# Longest consecutive-run: [5, 4] and [2, 1].

longest_run([3, 5, 7, 10, 15]) ➞ 1
# No consecutive runs, so we return 1.
```
## Notes

If there aren't any consecutive runs (there is a gap between each integer), return 1.

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


def longest_run(numbers: list[int]) -> int:
    return 0  # Put your code here!!!


test(747, longest_run)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                3,
                5,
                6,
                10,
                15
            ]
        ],
        "return": 2
    },
    {
        "args": [
            [
                1,
                2,
                3,
                2,
                1
            ]
        ],
        "return": 3
    },
    {
        "args": [
            [
                1,
                2,
                3,
                5,
                6,
                7,
                8,
                9
            ]
        ],
        "return": 5
    },
    {
        "args": [
            [
                5,
                4,
                2,
                1
            ]
        ],
        "return": 2
    },
    {
        "args": [
            [
                -7,
                -6,
                -5,
                -4,
                -3,
                -2,
                -1
            ]
        ],
        "return": 7
    }
]
```

## Credits

Found on Edabit: [Longest Consecutive Run](https://edabit.com/challenge/X9CsA6955cKRApBNH)
