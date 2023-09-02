# Challenge 742 - Current Streak

Create a function that takes the current day (e.g. `"2019-09-30"`), a list of date dictionaries and returns the "current streak" (i.e. number of consecutive days in a row ending on today).

## Examples
```python
current_streak("2019-09-23", [
  {
    "date": "2019-09-18"
  },
  {
    "date": "2019-09-19"
  },
  {
    "date": "2019-09-21"
  },
  {
    "date": "2019-09-22"
  },
  {
    "date": "2019-09-23"
  }
]) ➞ 3

current_streak("2019-09-25", [
  {
    "date": "2019-09-16"
  },
  {
    "date": "2019-09-17"
  },
  {
    "date": "2019-09-21"
  },
  {
    "date": "2019-09-22"
  },
  {
    "date": "2019-09-23"
  }
]) ➞ 0
```
## Notes

- The list of dates is sorted chronologically.
- The today parameter will always be greater than or equal to the last date in the list.
- An empty list should return 0.

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
from typing import TypeVar, TypedDict


Date = TypedDict("Date", {"date": str})


def current_streak(current_date: str, dates: list[Date]) -> int:
    return 0  # Put your code here!!!


test(742, current_streak)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            "2019-09-23",
            [
                {
                    "date": "2019-09-18"
                },
                {
                    "date": "2019-09-19"
                },
                {
                    "date": "2019-09-20"
                },
                {
                    "date": "2019-09-21"
                },
                {
                    "date": "2019-09-22"
                },
                {
                    "date": "2019-09-23"
                }
            ]
        ],
        "return": 6
    },
    {
        "args": [
            "2019-09-25",
            [
                {
                    "date": "2019-09-16"
                },
                {
                    "date": "2019-09-17"
                },
                {
                    "date": "2019-09-21"
                },
                {
                    "date": "2019-09-22"
                },
                {
                    "date": "2019-09-23"
                }
            ]
        ],
        "return": 0
    },
    {
        "args": [
            "2019-09-16",
            []
        ],
        "return": 0
    },
    {
        "args": [
            "1985-03-19",
            [
                {
                    "date": "1985-03-19"
                }
            ]
        ],
        "return": 1
    },
    {
        "args": [
            "2019-09-23",
            [
                {
                    "date": "2019-09-18"
                },
                {
                    "date": "2019-09-19"
                },
                {
                    "date": "2019-09-21"
                },
                {
                    "date": "2019-09-22"
                },
                {
                    "date": "2019-09-23"
                }
            ]
        ],
        "return": 3
    }
]
```

## Credits

Found on Edabit: [Current Streak](https://edabit.com/challenge/dHGpjWHJ265BCthiM)
