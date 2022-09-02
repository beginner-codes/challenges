# Challenge 530 - Number of Boomerangs 

A boomerang is a V-shaped sequence that is either upright or upside down. Specifically, a boomerang can be defined as: sub-list of length 3, with the first and last digits being the same and the middle digit being different.

Some boomerang examples:
```python
[3, 7, 3], [1, -1, 1], [5, 6, 5]
```
Create a function that returns the total number of boomerangs in a list.

To illustrate:
```python
[3, 7, 3, 2, 1, 5, 1, 2, 2, -2, 2]
# 3 boomerangs in this sequence:  [3, 7, 3], [1, 5, 1], [2, -2, 2]
```
Be aware that boomerangs can overlap, like so:
```python
[1, 7, 1, 7, 1, 7, 1]
# 5 boomerangs (from left to right): [1, 7, 1], [7, 1, 7], [1, 7, 1], [7, 1, 7], and [1, 7, 1]
```
## Examples
```python
count_boomerangs([9, 5, 9, 5, 1, 1, 1]) ➞ 2

count_boomerangs([5, 6, 6, 7, 6, 3, 9]) ➞ 1

count_boomerangs([4, 4, 4, 9, 9, 9, 9]) ➞ 0
```
## Notes

- `[5, 5, 5]` (triple identical digits) is NOT considered a boomerang because the middle digit is identical to the first and last.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def longest_zero(string: str) -> str:
    return "" # Put your code here!!!


test(529, longest_zero)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                1,
                7,
                1,
                7,
                1,
                7,
                1
            ]
        ],
        "return": 5
    },
    {
        "args": [
            [
                1,
                2,
                1,
                1,
                1,
                2,
                1
            ]
        ],
        "return": 2
    },
    {
        "args": [
            [
                4,
                4,
                4,
                9,
                9,
                9,
                9
            ]
        ],
        "return": 0
    },
    {
        "args": [
            [
                5,
                5,
                5
            ]
        ],
        "return": 0
    },
    {
        "args": [
            [
                9,
                5,
                9,
                5,
                1,
                1,
                1
            ]
        ],
        "return": 2
    }
]
```
## Credits

Found on Edabit: [Number of Boomerangs](https://edabit.com/challenge/25zkiePFYRpickxnB)
