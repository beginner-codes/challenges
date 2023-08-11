# Challenge 725 - Filter Primes from a List

Create a function that takes a list and returns a new list containing only prime numbers.

## Examples
```python
filter_primes([7, 9, 3, 9, 10, 11, 27]) ➞ [7, 3, 11]

filter_primes([10007, 1009, 1007, 27, 147, 77, 1001, 70]) ➞ [10007, 1009]

filter_primes([1009, 10, 10, 10, 3, 33, 9, 4, 1, 61, 63, 69, 1087, 1091, 1093, 1097]) ➞ [1009, 3, 61, 1087, 1091, 1093, 1097]
```
## Notes

- New list must maintain the order of primes as they first appear in the original list.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def filter_primes(numbers: list[int]) -> list[int]:
    return []  # Put your code here!!!


test(725, filter_primes)  # Tell it which challenge to test against
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
                4,
                5,
                6,
                7,
                8,
                9,
                10,
                11,
                12,
                13,
                14,
                15,
                16,
                17,
                18,
                19,
                20,
                21,
                22,
                23,
                24,
                25
            ]
        ],
        "return": [
            2,
            3,
            5,
            7,
            11,
            13,
            17,
            19,
            23
        ]
    },
    {
        "args": [
            [
                10007,
                1009,
                1007,
                27,
                147,
                77,
                1001,
                70
            ]
        ],
        "return": [
            10007,
            1009
        ]
    },
    {
        "args": [
            [
                7,
                9,
                3,
                9,
                10,
                11,
                27
            ]
        ],
        "return": [
            7,
            3,
            11
        ]
    },
    {
        "args": [
            [
                1009,
                10,
                10,
                10,
                3,
                33,
                9,
                4,
                1,
                61,
                63,
                69,
                1087,
                1091,
                1093,
                1097
            ]
        ],
        "return": [
            1009,
            3,
            61,
            1087,
            1091,
            1093,
            1097
        ]
    }
]
```
## Credits

Found on Edabit: [Filter Primes from a List](https://edabit.com/challenge/yXZhG7zq6dWhWhirt)
