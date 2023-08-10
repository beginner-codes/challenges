# Challenge 724 - Positive Count / Negative Sum

Create a function that takes a list of positive and negative numbers. Return a list where the first element is the count of positive numbers and the second element is the sum of negative numbers.

## Examples
```python
sum_neg([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, -11, -12, -13, -14, -15]) ➞ [10, -65]
# There are a total of 10 positive numbers.
# The sum of all negative numbers equals -65.

sum_neg([92, 6, 73, -77, 81, -90, 99, 8, -85, 34]) ➞ [7, -252]

sum_neg([91, -4, 80, -73, -28]) ➞ [2, -105]

sum_neg([]) ➞ []
```
## Notes

- If given an empty list, return an empty list
- 0 is not positive.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def sum_neg(numbers: list[int]) -> list[int]:
    return []  # Put your code here!!!


test(724, sum_neg)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                92,
                6,
                73,
                -77,
                81,
                -90,
                99,
                8,
                -85,
                34
            ]
        ],
        "return": [
            7,
            -252
        ]
    },
    {
        "args": [
            [
                98,
                51,
                -19,
                -97
            ]
        ],
        "return": [
            2,
            -116
        ]
    },
    {
        "args": [
            [
                5,
                7,
                9,
                -3,
                -7,
                61,
                -24
            ]
        ],
        "return": [
            4,
            -34
        ]
    },
    {
        "args": [
            [
                -42,
                3,
                -51,
                -64,
                69,
                77,
                -20,
                -5,
                68,
                -76
            ]
        ],
        "return": [
            4,
            -258
        ]
    },
    {
        "args": [
            []
        ],
        "return": []
    }
]
```
## Credits

Found on Edabit: [Positive Count / Negative Sum](https://edabit.com/challenge/RTZRnXCJkfALTTdqt)
