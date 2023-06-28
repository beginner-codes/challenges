# Challenge 694 - Consecutive Sum Check

Create a function that a number as an argument and checks whether the given number can be expressed as the sum of two or more consecutive positive numbers.

## Examples
```python
consecutive_sum(9) ➞ True
# 9 can be expressed as a sum of (2 + 3 + 4) or (4 + 5).

consecutive_sum(10) ➞ True
# 10 can be expressed as a sum of 1 + 2 + 3 + 4.

consecutive_sum(64) ➞ False
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def consecutive_sum(number: int) -> bool:
    return False  # Put your code here!!!


test(694, consecutive_sum)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            32
        ],
        "return": false
    },
    {
        "args": [
            13
        ],
        "return": true
    },
    {
        "args": [
            161997
        ],
        "return": true
    },
    {
        "args": [
            6
        ],
        "return": true
    },
    {
        "args": [
            323744
        ],
        "return": true
    }
]
```
## Credits

Found on Edabit: [Consecutive Sum Check](https://edabit.com/challenge/srEFhCNueikMKs3oT)
