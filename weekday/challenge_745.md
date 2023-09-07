# Challenge 745 - Sum of a List of Times

Create a function that takes a list of strings representing times (`'hours:minutes:seconds'`) and returns their sum as a list of integers (`[hours, minutes, seconds]`).

## Examples
```python
time_sum(["1:23:45"]) ➞ [1, 23, 45]

time_sum(["1:03:45", "1:23:05"]) ➞ [2, 26, 50]

time_sum(["5:39:42", "10:02:08", "8:26:33"]) ➞ [24, 8, 23]
```
## Notes

- If the input is an empty list, return `[0, 0, 0]`

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


def time_sum(times: list[str]) -> list[int]:
    return []  # Put your code here!!!


test(745, time_sum)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            []
        ],
        "return": [
            0,
            0,
            0
        ]
    },
    {
        "args": [
            [
                "5:39:42",
                "10:02:08",
                "8:26:33"
            ]
        ],
        "return": [
            24,
            8,
            23
        ]
    },
    {
        "args": [
            [
                "1:03:45",
                "1:23:05"
            ]
        ],
        "return": [
            2,
            26,
            50
        ]
    },
    {
        "args": [
            [
                "1:23:45",
                "0:00:00"
            ]
        ],
        "return": [
            1,
            23,
            45
        ]
    },
    {
        "args": [
            [
                "10:11:02",
                "8:57:30",
                "10:58:56",
                "4:04:17",
                "3:01:13"
            ]
        ],
        "return": [
            37,
            12,
            58
        ]
    }
]
```

## Credits

Found on Edabit: [Sum of a List of Times](https://edabit.com/challenge/wyr9gCiBtFM7YLauK)
