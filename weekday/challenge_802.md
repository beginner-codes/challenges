# Challenge 802 - Collatz Conjecture

A Collatz sequence is generated as follows:
- Start with a positive number
- If it's even, halve it
- If it's odd, multiply it by three and add one
- Repeat the process with the resulting number

The Collatz Conjecture is that every sequence eventually reaches 1 (continuing past 1 just results in an endless repeat of the sequence 4, 2, 1).

The length of the sequence from starting number to 1 varies widely.

Create a function that takes a number as an argument and returns a list of two elements — the number of steps in the Collatz sequence of the number, and the highest number reached.

## Examples
```python
collatz(2) ➞ [2, 2]
# seq = [2, 1]

collatz(3) ➞ [8, 16]
# seq = [3, 10, 5, 16, 8, 4, 2, 1]

collatz(7) ➞ [17, 52]
# seq = [7, 22, 11, 34, 17, 52, 26, 13, 40, 20, 10, 5, 16, 8, 4, 2, 1]

collatz(8) ➞ [4, 8]
# seq = [8, 4, 2, 1]
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


def collatz(start: int) -> list[int]:
    return []  # Put your code here!!!


test(802, collatz)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            7
        ],
        "return": [
            17,
            52
        ]
    },
    {
        "args": [
            33
        ],
        "return": [
            27,
            100
        ]
    },
    {
        "args": [
            17
        ],
        "return": [
            13,
            52
        ]
    },
    {
        "args": [
            3
        ],
        "return": [
            8,
            16
        ]
    },
    {
        "args": [
            42
        ],
        "return": [
            9,
            64
        ]
    }
]
```

## Credits

Found on Edabit: [Collatz Conjecture](https://edabit.com/challenge/Z8REdTE5P57f4q7dK)
