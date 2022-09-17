# Challenge 538 - Palindrome Sequence

A palindrome is a number that is the same when reversed, `2770772` for example. A palindrome can often be formed by adding a number to it's reverse: `641 + 146 = 787` (a palindrome). Using `78` as the seed, it takes 4 steps to produce a palindrome:
```python
78 + 87 = 165
165 + 561 = 726
726 + 627 = 1353
1353 + 3531 = 4884 (a palindrome)
```
About 97% of integers less than 10,000 produce palindromes in less than 25 steps. A few, like 196 and 879, may never form palindromes.

Make a function that takes a palindrome as its argument and returns the smallest seed integer that will produce that palindrome, along with the number of steps required:
```python
pal_seq(4884) ➞ (69, 4)

pal_seq(1) ➞ (1, 0)

pal_seq(11) ➞ (10, 1)
# 10 + 01 = 11

pal_seq(3113) ➞ (199, 3)

pal_seq(8836886388) ➞ (177, 15)
```
## Notes

- The sequence always terminates when the first palindrome is produced. If the seed is a palindrome, the sequence has 0 steps.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def pal_seq(palindrome: int) -> list[int, int]:
    return [0, 0] # Put your code here!!!


test(538, pal_seq)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            8813200023188
        ],
        "return": [
            89,
            24
        ]
    },
    {
        "args": [
            7777
        ],
        "return": [
            709,
            2
        ]
    },
    {
        "args": [
            52788725
        ],
        "return": [
            1894,
            13
        ]
    },
    {
        "args": [
            229922
        ],
        "return": [
            1079,
            6
        ]
    },
    {
        "args": [
            11
        ],
        "return": [
            10,
            1
        ]
    }
]
```
## Credits

Found on Edabit: [Palindrome Sequence](https://edabit.com/challenge/CYReZKzYxNBDs7Kce)
