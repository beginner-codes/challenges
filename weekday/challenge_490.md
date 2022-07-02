# Challenge 490 - Cinemas in 2021

Given a list of seats, return the maximum number of new people which can be seated, as long as there is at least a gap of 2 seats between people.

- Empty seats are given as `0`.
- Occupied seats are given as `1`.
- Don't move any seats which are already occupied, even if they are less than 2 seats apart. Consider only the gaps between new seats and existing seats.

## Examples
```python
maximum_seating([0, 0, 0, 1, 0, 0, 1, 0, 0, 0]) ➞ 2
# [1, 0, 0, 1, 0, 0, 1, 0, 0, 1]

maximum_seating([0, 0, 0, 0]) ➞ 2
# [1, 0, 0, 1]

maximum_seating([1, 0, 0, 0, 0, 1]) ➞ 0
# There is no way to have a gap of at least 2 chairs when adding someone else.
```
## Notes

- Notice how there may be several possibilities for assigning seats to people, but these cases won't affect the results.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def maximum_seating(seats: list[int]) -> int:
    return 0  # Put your code here!!!


test(490, maximum_seating)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                0,
                0,
                0,
                1,
                0,
                0,
                1,
                0,
                0,
                0
            ]
        ],
        "return": 2
    },
    {
        "args": [
            [
                0,
                0,
                0,
                0
            ]
        ],
        "return": 2
    },
    {
        "args": [
            [
                1,
                0,
                0,
                0,
                0,
                0,
                1
            ]
        ],
        "return": 1
    },
    {
        "args": [
            [
                1,
                0,
                0,
                0,
                0,
                0,
                0,
                1
            ]
        ],
        "return": 1
    },
    {
        "args": [
            [
                1,
                0,
                0,
                0,
                0,
                1
            ]
        ],
        "return": 0
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
                0,
                0,
                0,
                0
            ]
        ],
        "return": 4
    },
    {
        "args": [
            [
                0
            ]
        ],
        "return": 1
    },
    {
        "args": [
            [
                0,
                0
            ]
        ],
        "return": 1
    },
    {
        "args": [
            [
                1
            ]
        ],
        "return": 0
    },
    {
        "args": [
            [
                0,
                1,
                0,
                0,
                0,
                1,
                1,
                0,
                0,
                0,
                0,
                1,
                1,
                0,
                0,
                1,
                0,
                1,
                1,
                0,
                1,
                1,
                0,
                0,
                0,
                0
            ]
        ],
        "return": 1
    }
]
```
## Credits

Found on Edabit: [Cinemas in 2021](https://edabit.com/challenge/4xZFisQX8NnYB3nv4)
