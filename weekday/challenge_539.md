# Challenge 539 - Number Length Sort

Create a sorting function which sorts numbers not by numerical order, but by number length! This means sorting numbers with the least digits first, up to the numbers with the most digits.

## Examples
```python
number_len_sort([1, 54, 1, 2, 463, 2]) ➞ [1, 1, 2, 2, 54, 463]

number_len_sort([999, 421, 22, 990, 32]) ➞ [22, 32, 999, 421, 990]

number_len_sort([9, 8, 7, 6, 5, 4, 31, 2, 1, 3]) ➞ [9, 8, 7, 6, 5, 4, 2, 1, 3, 31]
```
## Notes

- If two numbers have the same number of digits, return them in the order they first appeared (this makes it different to just sorting the numbers normally).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def number_len_sort(numbers: list[int]) -> list[int]:
    return [] # Put your code here!!!


test(539, number_len_sort)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                3940,
                4334
            ]
        ],
        "return": [
            3940,
            4334
        ]
    },
    {
        "args": [
            [
                8013,
                1753,
                7283,
                6830,
                73,
                6278,
                4931,
                4556
            ]
        ],
        "return": [
            73,
            8013,
            1753,
            7283,
            6830,
            6278,
            4931,
            4556
        ]
    },
    {
        "args": [
            [
                4038,
                4156
            ]
        ],
        "return": [
            4038,
            4156
        ]
    },
    {
        "args": [
            [
                1321,
                7671,
                4235,
                5989
            ]
        ],
        "return": [
            1321,
            7671,
            4235,
            5989
        ]
    },
    {
        "args": [
            [
                5429,
                274,
                256,
                3437,
                3222,
                3294,
                5648,
                3281,
                6696,
                1883
            ]
        ],
        "return": [
            274,
            256,
            5429,
            3437,
            3222,
            3294,
            5648,
            3281,
            6696,
            1883
        ]
    }
]
```
## Credits

Found on Edabit: [Number Length Sort](https://edabit.com/challenge/Fx7hyoNTZNMGzc3uj)
