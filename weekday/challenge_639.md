# Challenge 639 - Primorial of a Number

In mathematics, primorial is a function from natural numbers to natural numbers similar to the factorial function. Rather than successively multiplying positive integers, the function only multiplies prime numbers.

Create a function that takes an integer and returns its primorial.

## Examples
```python
primorial(1) ➞ 2
# First prime number = 2

primorial(2) ➞ 6
# Product of first two prime numbers = 2*3 = 6

primorial(6) ➞ 30030
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def primorial(n: int) -> int:
    return 0  # Put your code here!!!


test(639, primorial)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            3
        ],
        "return": 30
    },
    {
        "args": [
            9
        ],
        "return": 223092870
    },
    {
        "args": [
            5
        ],
        "return": 2310
    },
    {
        "args": [
            1
        ],
        "return": 2
    },
    {
        "args": [
            4
        ],
        "return": 210
    }
]
```
## Credits

Found on Edabit: [Primorial of a Number](https://edabit.com/challenge/czLhTsGjScMTDtZxJ)
