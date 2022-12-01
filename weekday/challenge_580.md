# Challenge 580 - Time Conversion

Write a function that takes the number of seconds and returns the digital format clock time as a string. Time should be counted from `00:00:00`.

## Examples
```python
digital_clock(5025) ➞ "01:23:45"
# 5025 seconds is 1 hour, 23 mins, 45 secs.

digital_clock(61201) ➞ "17:00:01"
# No AM/PM. 24h format.

digital_clock(87000) ➞ "00:10:00"
# It's 00:10 next day.
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def digital_clock(seconds: int) -> str:
    return ""  # Put your code here!!!


test(580, digital_clock)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            61201
        ],
        "return": "17:00:01"
    },
    {
        "args": [
            40271
        ],
        "return": "11:11:11"
    },
    {
        "args": [
            4666
        ],
        "return": "01:17:46"
    },
    {
        "args": [
            86399
        ],
        "return": "23:59:59"
    },
    {
        "args": [
            87000
        ],
        "return": "00:10:00"
    }
]
```
## Credits

Found on Edabit: [Time Conversion](https://edabit.com/challenge/LgvppFDZoMpBKf8JW)
