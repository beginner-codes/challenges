# Challenge 705 - Up the Hill, Down the Hill

If a person traveled up a hill for 18 minutes at 20mph and then traveled back down the same path at 60mph then their average speed traveled was 30mph.

Write a function that returns the average speed traveled given an uphill time, uphill rate and a downhill rate. Uphill time is given in minutes. Return the rate as an integer (mph). No rounding is necessary.

## Examples
```python
avg_speed(18, 20, 60) ➞ 30

avg_speed(30, 10, 30) ➞ 15

avg_speed(30, 8, 24) ➞ 12
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def avg_speed(time: int, uphill_rate: int, downhill_rate: int) -> int:
    return 0  # Put your code here!!!


test(705, avg_speed)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            30,
            8,
            24
        ],
        "return": 12
    },
    {
        "args": [
            30,
            10,
            30
        ],
        "return": 15
    },
    {
        "args": [
            18,
            20,
            60
        ],
        "return": 30
    },
    {
        "args": [
            18,
            10,
            30
        ],
        "return": 15
    }
]
```
## Credits

Found on Edabit: [Up the Hill, Down the Hill](https://edabit.com/challenge/NYEaXXCnSj9jteNWA)
