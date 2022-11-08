# Challenge 568 - Days in a Month

Create a function that takes the month and year (as integers) and returns the number of days in that month.

## Examples
```python
days_in_month(2, 2018) ➞ 28

days_in_month(4, 654) ➞ 30

days_in_month(2, 200) ➞ 28

days_in_month(2, 1000) ➞ 28
```
## Notes

- Don't forget about leap years!

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def days_in_month(month: int, year: int) -> int:
    return 0 # Put your code here!!!


test(568, days_in_month)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            8,
            2018
        ],
        "return": 31
    },
    {
        "args": [
            10,
            2018
        ],
        "return": 31
    },
    {
        "args": [
            4,
            2018
        ],
        "return": 30
    },
    {
        "args": [
            2,
            2018
        ],
        "return": 28
    },
    {
        "args": [
            2,
            1600
        ],
        "return": 29
    }
]
```
## Credits

Found on Edabit: [Days in a Month](https://edabit.com/challenge/XZQw3zto7keDWPa5v)
