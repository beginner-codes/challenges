# Challenge 576 - When to Sleep?

Given a series of lists, with each individual list containing the time the alarm was set for followed by the amount of time that was spent sleeping, return what time they went to bed.

## Examples
```python
bed_time(["07:50", "07:50"]) ➞ ["00:00"]
# The second argument means 7 hours, 50 minutes sleep duration.

bed_time(["06:15", "10:00"], ["08:00", "10:00"], ["09:30", "10:00"]) ➞ ["20:15", "22:00", "23:30"]
# The second argument of each sub list means 10 hours sleep duration.

bed_time(["05:45", "04:00"], ["07:10", "04:30"]) ➞ ["01:45", "02:40"]
# Sleep duration can be different among the lists.
```
## Notes

- Times should be given in 24-hrs (i.e. `"23:25"` as opposed to `"11:25PM"`).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def bed_time(*records: list[str]) -> list[str]:
    return []  # Put your code here!!!


test(576, bed_time)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "05:45",
                "04:00"
            ],
            [
                "07:10",
                "04:30"
            ]
        ],
        "return": [
            "01:45",
            "02:40"
        ]
    },
    {
        "args": [
            [
                "07:50",
                "07:50"
            ]
        ],
        "return": [
            "00:00"
        ]
    },
    {
        "args": [
            [
                "06:15",
                "10:00"
            ],
            [
                "08:00",
                "10:00"
            ],
            [
                "09:30",
                "10:00"
            ]
        ],
        "return": [
            "20:15",
            "22:00",
            "23:30"
        ]
    }
]
```
## Credits

Found on Edabit: [When to Sleep?](https://edabit.com/challenge/e5XZ82bAk2rBo9EfS)
