# Challenge 578 - Numbers Transformation

You are given two positive integers `n` and `m`. You have to perform some basic mathematical operations on `n` to obtain `m`. These are your options:
```
(n-1)/2   - if (n-1) is divisible by 2
n/2       - if n is divisible by 2
n*2
```
Create a function that returns the minimum number of steps required to transform n into m.

## Examples
```javascript
number_transform(2, 8) ➞ 2
// 2 * 2 = 4
// 4 * 2 = 8

number_transform(9, 2) ➞ 2
// (9-1) / 2 = 4
// 4 / 2 = 2

number_transform(1024, 1024) ➞ 0
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def number_transform(n: int, m: int) -> int:
    return 0  # Put your code here!!!


test(578, number_transform)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            4,
            1
        ],
        "return": 2
    },
    {
        "args": [
            4096,
            1
        ],
        "return": 12
    },
    {
        "args": [
            1,
            4
        ],
        "return": 2
    },
    {
        "args": [
            2048,
            2
        ],
        "return": 10
    },
    {
        "args": [
            2,
            4
        ],
        "return": 1
    }
]
```
## Credits

Found on Edabit: [Numbers Transformation](https://edabit.com/challenge/bH5qdje5xgTYn4ypJ)
