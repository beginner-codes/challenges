# Challenge 777 - Esthetic Numbers

A number is Esthetic if, in any base from base2 up to base10, the absolute difference between every pair of its adjacent digits is constantly equal to 1.
```python
num = 441 (base10)
# Adjacent pairs of digits:
# |4, 4|, |4, 1|
# The absolute difference is not constant
# 441 is not Esthetic in base10

441 in base4 = 12321
# Adjacent pairs of digits:
# |1, 2|, |2, 3|, |3, 2|, |2, 1|
# The absolute difference is constant and is equal to 1
# 441 is Esthetic in base4
```
Given a positive integer, implement a function that returns a list containing the bases (as integers from 2 up to 10) in which number is found to be esthetic.

## Examples
```python
esthetic_bases(10) ➞ [2, 3, 8, 10]
# 10 in base2 = 1010
# 10 in base3 = 101
# 10 in base8 = 12
# 10 in base10 = 10

esthetic_bases(23) ➞ [3, 5, 7, 10]
# 23 in base3 = 212
# 23 in base5 = 43
# 23 in base7 = 32
# 23 in base10 = 23

esthetic_bases(666) ➞ [8]
# 666 in base8 = 1232 
```
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


def esthetic_bases(number: int) -> list[int]:
    return []  # Put your code here!!!


test(777, esthetic_bases)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            1080899
        ],
        "return": []
    },
    {
        "args": [
            74
        ],
        "return": []
    },
    {
        "args": [
            666
        ],
        "return": [
            8
        ]
    },
    {
        "args": [
            10
        ],
        "return": [
            2,
            3,
            8,
            10
        ]
    },
    {
        "args": [
            9
        ],
        "return": [
            4,
            7,
            9,
            10
        ]
    }
]
```

## Credits

Found on Edabit: [Esthetic](https://edabit.com/challenge/ruPm4LX6fEvvLJk9j)
