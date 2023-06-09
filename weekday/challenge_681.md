# Challenge 681 - Weekly Salary

Write a function that takes a list of hours and returns the total weekly salary.

The input list hours is listed sequentially, ordered from Monday to Sunday.

- A worker earns $10 an hour for the first 8 hours.
- For every overtime hour, he earns $15.
- On weekends, the employer pays double the usual rate, regardless of how many hours were already worked that week. For instance, 10 hours worked on a weekday would pay `80+30 = $110`, but on a weekend it would pay `160+60 = $220`.

## Examples
```python
weekly_salary([8, 8, 8, 8, 8, 0, 0]) ➞ 400

weekly_salary([10, 10, 10, 0, 8, 0, 0]) ➞ 410

weekly_salary([0, 0, 0, 0, 0, 12, 0]) ➞ 280
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def weekly_salary(hours: list[int]) -> int:
    return 0  # Put your code here!!!


test(681, weekly_salary)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                8,
                8,
                8,
                8,
                8,
                8,
                0
            ]
        ],
        "return": 560
    },
    {
        "args": [
            [
                8,
                8,
                8,
                8,
                8,
                8,
                8
            ]
        ],
        "return": 720
    },
    {
        "args": [
            [
                0,
                12,
                0,
                12,
                0,
                8,
                8
            ]
        ],
        "return": 600
    },
    {
        "args": [
            [
                1,
                1,
                1,
                2,
                5,
                0,
                0
            ]
        ],
        "return": 100
    },
    {
        "args": [
            [
                0,
                0,
                0,
                0,
                0,
                16,
                0
            ]
        ],
        "return": 400
    },
    {
        "args": [
            [
                10,
                10,
                10,
                10,
                10,
                10,
                10
            ]
        ],
        "return": 990
    },
    {
        "args": [
            [
                0,
                0,
                0,
                0,
                0,
                0,
                0
            ]
        ],
        "return": 0
    }
]
```
## Credits

Found on Edabit: [Weekly Salary](https://edabit.com/challenge/5uMJmbN2uihcyEu75)
