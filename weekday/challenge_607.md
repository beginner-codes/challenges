# Challenge 607 - Trailing Zeros

Create a function which takes a number and calculates how many trailing zeros the factorial of the number has.
```
n! = 1 * 2 * 3 * ... * n
```
## Examples
```python
trailing_zeros(0) ➞ 0
# 0! = 1
# No trailing zero.

trailing_zeros(6) ➞ 1
# 6! = 720
# 1 trailing zero.

trailing_zeros(1000) ➞ 249
# 1000! has 249 trailing zeros.
```
## Notes

- Hint: No need to calculate the factorial (because it won't help). Find another way to find the number of zeros.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def trailing_zeros(number: int) -> int:
    return 0  # Put your code here!!!


test(607, trailing_zeros)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            100000
        ],
        "return": 24999
    },
    {
        "args": [
            6
        ],
        "return": 1
    },
    {
        "args": [
            100
        ],
        "return": 24
    },
    {
        "args": [
            1000000000
        ],
        "return": 249999998
    },
    {
        "args": [
            30
        ],
        "return": 7
    }
]
```
## Credits

Found on Edabit: [Trailing Zeros](https://edabit.com/challenge/q7rHnH9Jhf35NqSjG)
