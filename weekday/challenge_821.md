# Challenge 821 - Get the Date

Write a function that, given a date (in the format `MM/DD/YYYY`), returns the day of the week as a string. Each day name must be one of the following strings: `"Sunday"`, `"Monday"`, `"Tuesday"`, `"Wednesday"`, `"Thursday"`, `"Friday"`, or `"Saturday"`.

To illustrate, the day of the week for `"12/07/2016"` is `"Wednesday"`.

## Examples
```python
get_day("12/07/2016") ➞ "Wednesday"

get_day("09/04/2016") ➞ "Sunday"

get_day("12/08/2011") ➞ "Thursday"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. *
*[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a
key `args` that are a list of parameters your function should take. The `return` key is what your function should return
given the `args`.

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your
solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:

```python
from __future__ import annotations
from beginnercodes.challenges import test


def get_day(date: str) -> str:
    return ""  # Put your code here!!!


test(821, get_day)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            "09/04/2016"
        ],
        "return": "Sunday"
    },
    {
        "args": [
            "06/08/2012"
        ],
        "return": "Friday"
    },
    {
        "args": [
            "12/08/2011"
        ],
        "return": "Thursday"
    },
    {
        "args": [
            "08/13/2019"
        ],
        "return": "Tuesday"
    },
    {
        "args": [
            "12/07/2016"
        ],
        "return": "Wednesday"
    }
]
```

## Credits

Found on Edabit: [Get the Date](https://edabit.com/challenge/3oqStN7bevcT72fgk)
