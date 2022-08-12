# Challenge 517 - Primes Below a Given Number

Create a function that will find all primes below a given number. Return the result as a list.

## Examples
```python
primes_below_num(5) ➞ [2, 3, 5]

primes_below_num(10) ➞ [2, 3, 5, 7]

primes_below_num(20) ➞ [2, 3, 5, 7, 11, 13, 17, 19]
```
## Notes

- If `n` is a prime, include it in the list.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def primes_below_num(number: int) -> list[int]:
    return [] # Put your code here!!!


test(517, primes_below_num)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            5
        ],
        "return": [
            2,
            3,
            5
        ]
    },
    {
        "args": [
            8
        ],
        "return": [
            2,
            3,
            5,
            7
        ]
    },
    {
        "args": [
            7
        ],
        "return": [
            2,
            3,
            5,
            7
        ]
    },
    {
        "args": [
            12
        ],
        "return": [
            2,
            3,
            5,
            7,
            11
        ]
    },
    {
        "args": [
            13
        ],
        "return": [
            2,
            3,
            5,
            7,
            11,
            13
        ]
    }
]
```
## Credits

Found on Edabit: [Primes Below a Given Number](https://edabit.com/challenge/SFAjxGWk9AbfwbXFN)
