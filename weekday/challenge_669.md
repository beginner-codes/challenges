# Challenge 669 - LCM of Two Numbers

Write a function that returns the least common multiple (LCM) of two integers.

## Examples
```python
lcm(9, 18) ➞ 18

lcm(8, 5) ➞ 40

lcm(17, 11) ➞ 187
```
## Notes

- Both values will be positive.
- The LCM is the smallest integer that is divisible by both numbers such that the remainder is zero.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def lcm(number_a: int, number_b: int) -> int:
    return 0  # Put your code here!!!


test(669, lcm)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            8,
            5
        ],
        "return": 40
    },
    {
        "args": [
            9,
            9
        ],
        "return": 9
    },
    {
        "args": [
            9,
            18
        ],
        "return": 18
    },
    {
        "args": [
            3,
            12
        ],
        "return": 12
    },
    {
        "args": [
            17,
            11
        ],
        "return": 187
    },
    {
        "args": [
            17,
            5
        ],
        "return": 85
    }
]
```
## Credits

Found on Edabit: [LCM of Two Numbers](https://edabit.com/challenge/rSa8y4gxJtBqbMrPW)
