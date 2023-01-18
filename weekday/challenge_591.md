# Challenge 591 - Inclusive List Ranges

Write a function that, given the start and end values, return a list containing all the numbers inclusive to that range.

## Examples
```python
inclusive_list(1, 5) ➞ [1, 2, 3, 4, 5]

inclusive_list(2, 8) ➞ [2, 3, 4, 5, 6, 7, 8]

inclusive_list(10, 20) ➞ [10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20]

inclusive_list(17, 5) ➞ [17]
```
## Notes

- The numbers in the list are sorted in ascending order.
- If the start is greater than the end, return a list with the higher value.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def inclusive_list(start: int, end: int) -> list[int]:
    return []  # Put your code here!!!


test(591, inclusive_list)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            24,
            17
        ],
        "return": [
            24
        ]
    },
    {
        "args": [
            11,
            66
        ],
        "return": [
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
            25,
            26,
            27,
            28,
            29,
            30,
            31,
            32,
            33,
            34,
            35,
            36,
            37,
            38,
            39,
            40,
            41,
            42,
            43,
            44,
            45,
            46,
            47,
            48,
            49,
            50,
            51,
            52,
            53,
            54,
            55,
            56,
            57,
            58,
            59,
            60,
            61,
            62,
            63,
            64,
            65,
            66
        ]
    },
    {
        "args": [
            6,
            16
        ],
        "return": [
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
            16
        ]
    },
    {
        "args": [
            40,
            50
        ],
        "return": [
            40,
            41,
            42,
            43,
            44,
            45,
            46,
            47,
            48,
            49,
            50
        ]
    },
    {
        "args": [
            17,
            5
        ],
        "return": [
            17
        ]
    }
]
```
## Credits

Found on Edabit: [Inclusive List Ranges](https://edabit.com/challenge/bHTb8p5nybCrjFPze)
