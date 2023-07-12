# Challenge 703 - Hours Passed

Create a function that takes two times and returns how many hours have passed between them.

## Examples
```python
hours_passed("3:00 AM", "9:00 AM") ➞ "6 hours"

hours_passed("2:00 PM", "4:00 PM") ➞ "2 hours"

hours_passed("1:00 AM", "3:00 PM") ➞ "14 hours"
```
## Notes

- The first time will always be the starting time and second the ending time.
- Return `"no time passed"` if the two times are equal.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def hours_past(time1: str, time2: str) -> str:
    return ""  # Put your code here!!!


test(703, hours_past)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "12:00 PM",
            "12:00 PM"
        ],
        "return": "no time passed"
    },
    {
        "args": [
            "2:00 AM",
            "3:00 PM"
        ],
        "return": "13 hours"
    },
    {
        "args": [
            "3:00 AM",
            "9:00 AM"
        ],
        "return": "6 hours"
    },
    {
        "args": [
            "1:00 AM",
            "1:00 AM"
        ],
        "return": "no time passed"
    },
    {
        "args": [
            "1:00 AM",
            "3:00 PM"
        ],
        "return": "14 hours"
    }
]
```
## Credits

Found on Edabit: [Hours Passed](https://edabit.com/challenge/cgyHTJDW5brpXGDy6)
