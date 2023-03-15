# Challenge 623 - Day Number of Year

Each year has 365 or 366 days. Given a string date representing a Gregorian calendar date formatted as month/day/year, return the day-number of the year.

## Examples
```python
day_of_year("11/16/2020") ➞ 321

day_of_year("1/9/2019") ➞ 9

day_of_year("3/1/2004") ➞ 61

day_of_year("12/31/2000") ➞ 366
```
## Notes

- All input strings in tests are valid dates.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def day_of_year(date: str) -> int:
    return 0  # Put your code here!!!


test(623, day_of_year)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "10/7/2050"
        ],
        "return": 280
    },
    {
        "args": [
            "3/1/2004"
        ],
        "return": 61
    },
    {
        "args": [
            "11/3/2020"
        ],
        "return": 308
    },
    {
        "args": [
            "5/3/0002"
        ],
        "return": 123
    },
    {
        "args": [
            "8/29/1900"
        ],
        "return": 241
    }
]
```
## Credits

Found on Edabit: [Day Number of Year](https://edabit.com/challenge/fTXXkQ7bfuQDjgNyH)
