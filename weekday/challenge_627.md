# Challenge 627 - Radians to Degrees

Create a function that takes an angle in radians and returns the corresponding angle in degrees rounded to one decimal place.

## Examples
```python
radians_to_degrees(1) ➞ 57.3

radians_to_degrees(20) ➞ 1145.9

radians_to_degrees(50) ➞ 2864.8
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def radians_to_degrees(degrees: int) -> float:
    return 0  # Put your code here!!!


test(627, radians_to_degrees)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            5
        ],
        "return": 286.5
    },
    {
        "args": [
            7
        ],
        "return": 401.1
    },
    {
        "args": [
            60
        ],
        "return": 3437.7
    },
    {
        "args": [
            180
        ],
        "return": 10313.2
    },
    {
        "args": [
            100
        ],
        "return": 5729.6
    },
    {
        "args": [
            1
        ],
        "return": 57.3
    }
]
```
## Credits

Found on Edabit: [Radians to Degrees](https://edabit.com/challenge/2X2uZysLJ3CpsxLDD)
