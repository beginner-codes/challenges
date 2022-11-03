# Challenge 564 - Generate a List of 15 Palindrome Numbers

In this challenge, you have to find the last 15 palindromes of all numbers starting from ten and up to a given limit, including the limit in the search.

Given an upper limit, implement a function that returns the last 15 numbers that are palindromes less than or equal to the limit. Return them as a list in ascending order.

## Examples
```python
generate_palindromes(151) ➞ [
  11, 22, 33, 44, 55,
  66, 77, 88, 99, 101,
  111, 121, 131, 141, 151
]

generate_palindromes(600) ➞ [
  454, 464, 474, 484, 494,
  505, 515, 525, 535, 545,
  555, 565, 575, 585, 595
]

generate_palindromes(999999) ➞ [
  985589, 986689, 987789, 988889, 989989,
  990099, 991199, 992299, 993399, 994499,
  995599, 996699, 997799, 998899, 999999
]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def generate_palindromes(max_num: int) -> list[int]:
    return [] # Put your code here!!!


test(564, generate_palindromes)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            600
        ],
        "return": [
            454,
            464,
            474,
            484,
            494,
            505,
            515,
            525,
            535,
            545,
            555,
            565,
            575,
            585,
            595
        ]
    },
    {
        "args": [
            3443
        ],
        "return": [
            2002,
            2112,
            2222,
            2332,
            2442,
            2552,
            2662,
            2772,
            2882,
            2992,
            3003,
            3113,
            3223,
            3333,
            3443
        ]
    },
    {
        "args": [
            13000
        ],
        "return": [
            11511,
            11611,
            11711,
            11811,
            11911,
            12021,
            12121,
            12221,
            12321,
            12421,
            12521,
            12621,
            12721,
            12821,
            12921
        ]
    },
    {
        "args": [
            999999
        ],
        "return": [
            985589,
            986689,
            987789,
            988889,
            989989,
            990099,
            991199,
            992299,
            993399,
            994499,
            995599,
            996699,
            997799,
            998899,
            999999
        ]
    },
    {
        "args": [
            151
        ],
        "return": [
            11,
            22,
            33,
            44,
            55,
            66,
            77,
            88,
            99,
            101,
            111,
            121,
            131,
            141,
            151
        ]
    }
]
```
## Credits

Found on Edabit: [Generate a List of 15 Palindrome Numbers](https://edabit.com/challenge/9QbhjtbkXp3QZNuDu)
