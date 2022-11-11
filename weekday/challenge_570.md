# Challenge 570 - Longest Daily Streak

Create a function that takes a list of booleans that represent whether a player has logged into a game that day. Output the longest streak of consecutive logged in days.

## Examples
```python
daily_streak([True, True, False, True]) ➞ 2

daily_streak([False, False, False]) ➞ 0

daily_streak([True, True, True, False, True, True]) ➞ 3
```
## Notes

- Return your output as an integer.
- If a given list is all `False`, return `0`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def daily_streak(days: list[bool]) -> int:
    return 0  # Put your code here!!!


test(570, daily_streak)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                true,
                false
            ]
        ],
        "return": 1
    },
    {
        "args": [
            [
                true,
                true,
                true,
                false
            ]
        ],
        "return": 3
    },
    {
        "args": [
            [
                true,
                false,
                true,
                true
            ]
        ],
        "return": 2
    },
    {
        "args": [
            [
                true,
                true,
                true,
                false,
                true,
                true
            ]
        ],
        "return": 3
    },
    {
        "args": [
            [
                true,
                false,
                true
            ]
        ],
        "return": 1
    }
]
```
## Credits

Found on Edabit: [Longest Daily Streak](https://edabit.com/challenge/sTJoRiHpQJvmqscGP)
