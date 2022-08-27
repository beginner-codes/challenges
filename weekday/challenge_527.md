# Challenge 527 - Summation of the First n Terms 

Create a function that takes an expression and an upper limit as arguments and return the sum of that expression up to the `i`th term.

## Examples
```python
summation("n", 10) ➞ 55

summation("1/n", 50) ➞ 4.5

summation("n**n", 6) ➞ 50069
```
## Notes

- Assume the lower limit is `i = 1`.
- Round your answer to the nearest tenth.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

def summation(expression: str, limit: int) -> int:
    return 0 # Put your code here!!!


test(527, summation)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "-n",
            100
        ],
        "return": -5050
    },
    {
        "args": [
            "1/n",
            50
        ],
        "return": 4.5
    },
    {
        "args": [
            "(2*n**2 + 5*n)/3",
            30
        ],
        "return": 7078.3
    },
    {
        "args": [
            "19",
            56
        ],
        "return": 1064
    },
    {
        "args": [
            "n",
            10
        ],
        "return": 55
    }
]
```
## Credits

Found on Edabit: [Summation of the First n Terms](https://edabit.com/challenge/Gdoh8rdoaB9jJLLAn)
