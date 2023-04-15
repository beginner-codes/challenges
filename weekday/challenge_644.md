# Challenge 644 - Prime Divisors

Create a function that takes a number as an argument and returns all of its prime divisors.

To illustrate:
> If n = 27
> All divisors are: `[3, 9, 27]`
> Finally, from that list of divisors, return the prime ones: `[3]`

## Examples
```python
prime_divisors(27) ➞ [3]

prime_divisors(99) ➞ [3, 11]

prime_divisors(3457) ➞ [3457]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def prime_divisors(number: int) -> list[int]:
    return []  # Put your code here!!!


test(644, prime_divisors)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            462
        ],
        "return": [
            2,
            3,
            7,
            11
        ]
    },
    {
        "args": [
            99
        ],
        "return": [
            3,
            11
        ]
    },
    {
        "args": [
            27
        ],
        "return": [
            3
        ]
    },
    {
        "args": [
            1386
        ],
        "return": [
            2,
            3,
            7,
            11
        ]
    },
    {
        "args": [
            24
        ],
        "return": [
            2,
            3
        ]
    },
    {
        "args": [
            478170
        ],
        "return": [
            2,
            3,
            5,
            7,
            11,
            23
        ]
    }
]
```
## Credits

Found on Edabit: [Prime Divisors](https://edabit.com/challenge/FbQqXepHC4wxrWgYg)
