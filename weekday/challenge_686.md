# Challenge 686 - Number Rounding 

Create a function that takes an integer number and an integer rounding factor and returns an integer which is divisible by the rounding factor and is the closest to the number. If there are two numbers equidistant from the number that are both divisible by the rounding factor, select the larger one.

## Examples
```python
round_number(33, 25) ➞ 25

round_number(46, 7) ➞ 49

round_number(133, 14) ➞ 140
```
## Notes

- The number will always be a positive.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def round_number(number: int, rounding_factor: int) -> int:
    return 0  # Put your code here!!!


test(686, round_number)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            6247,
            163
        ],
        "return": 6194
    },
    {
        "args": [
            642234,
            1523
        ],
        "return": 642706
    },
    {
        "args": [
            65,
            10
        ],
        "return": 70
    },
    {
        "args": [
            96623443,
            7650
        ],
        "return": 96627150
    },
    {
        "args": [
            532,
            12
        ],
        "return": 528
    }
]
```
## Credits

Found on Edabit: [Round to Closest N](https://edabit.com/challenge/zZyeau2MYcEc8Fdtk)
