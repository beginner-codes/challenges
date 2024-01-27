# Challenge 813 - Sort by Factor Length

A numbers factor length is simply its total number of factors.

For instance:
```python
3: 1, 3
# 3's factor length = 2

8: 1, 2, 4, 8
# 8's factor length = 4

36 : 1, 2, 3, 4, 6, 9, 12, 18, 36
# 36's factor length = 9
```
Create a function that sorts a list by factor length in descending order. If multiple numbers have the same factor length, sort these numbers in descending order, with the largest first.

In the example below, since 13 and 7 both have only 2 factors, we put 13 ahead of 7.
```python
factor_sort([9, 7, 13, 12]) ➞ [12, 9, 13, 7]
# 12 : 6, 9: 3, 13: 2, 7: 2
```
## Examples
```python
factor_sort([1, 2, 31, 4]) ➞ [4, 31, 2, 1]

factor_sort([5, 7, 9]) ➞ [9, 7, 5]

factor_sort([15, 8, 2, 3]) ➞ [15, 8, 3, 2]
```
## Notes

- Descending order: numbers with a higher factor length go before numbers with a lower factor length.

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


def factor_sort(numbers: list[int]) -> list[int]:
    return []  # Put your code here!!!


test(813, factor_sort)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                15,
                8,
                2,
                3
            ]
        ],
        "return": [
            15,
            8,
            3,
            2
        ]
    },
    {
        "args": [
            [
                1,
                2,
                3,
                7,
                11,
                13,
                16
            ]
        ],
        "return": [
            16,
            13,
            11,
            7,
            3,
            2,
            1
        ]
    },
    {
        "args": [
            [
                5,
                7,
                9
            ]
        ],
        "return": [
            9,
            7,
            5
        ]
    },
    {
        "args": [
            [
                1,
                2,
                31,
                4
            ]
        ],
        "return": [
            4,
            31,
            2,
            1
        ]
    },
    {
        "args": [
            [
                1,
                5,
                25,
                17
            ]
        ],
        "return": [
            25,
            17,
            5,
            1
        ]
    }
]
```

## Credits

Found on Edabit: [Sort by Factor Length](https://edabit.com/challenge/u9mxp7LLxogAjAGDN)
