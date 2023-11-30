# Challenge 803 - List of Prime Factors

Write a function that returns the extended form of the prime factorization of a number. Return in the format `[a, b, c, d, ...]`, where each element of the list is an integer.

## Examples
```python
prime_factorization(216) ➞ [2, 2, 2, 3, 3, 3]

prime_factorization(64) ➞ [2, 2, 2, 2, 2, 2]

prime_factorization(23) ➞ [23]
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


def prime_factorization(number: int) -> list[int]:
    return []  # Put your code here!!!


test(803, prime_factorization)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            1
        ],
        "return": []
    },
    {
        "args": [
            99
        ],
        "return": [
            3,
            3,
            11
        ]
    },
    {
        "args": [
            100
        ],
        "return": [
            2,
            2,
            5,
            5
        ]
    },
    {
        "args": [
            57
        ],
        "return": [
            3,
            19
        ]
    },
    {
        "args": [
            8
        ],
        "return": [
            2,
            2,
            2
        ]
    }
]
```

## Credits

Found on Edabit: [List of Prime Factors](https://edabit.com/challenge/QCgDtyfajCT4PGhFK)
