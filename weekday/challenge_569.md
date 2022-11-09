# Challenge 569 - Is There an Upward Trend?

Create a function that determines if there is an upward trend.

## Examples
```python
upward_trend([1, 2, 3, 4]) ➞ True

upward_trend([1, 2, 6, 5, 7, 8]) ➞ False

upward_trend([1, 2, 3, "4"]) ➞ "Strings not permitted!"

upward_trend([1, 2, 3, 6, 7]) ➞ True
```
## Notes

- If there is a string element in the list, return `"Strings not permitted!"`.
- The numbers don't have to be consecutive (e.g. `[1, 3, 5]` should still return `True`).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def upward_trend(numbers: list[int | str]) -> bool | str:
    return "" # Put your code here!!!


test(569, upward_trend)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                10,
                12,
                13,
                15,
                20
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                1,
                2,
                3,
                4,
                5,
                6
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                1,
                3,
                2,
                5,
                6,
                7
            ]
        ],
        "return": false
    },
    {
        "args": [
            [
                1,
                3,
                5,
                7,
                9
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                6,
                9,
                11,
                15,
                12
            ]
        ],
        "return": false
    }
]
```
## Credits

Found on Edabit: [Is There an Upward Trend?](https://edabit.com/challenge/nr35Bm5BRQYHZrt5n)
