# Challenge 662 - Dice Gambling

Create a function that takes a list consisting of dice rolls from 1-6. Return the sum of your rolls with the following conditions:

- If a 1 is rolled, that is bad luck. The next roll counts as 0.
- If a 6 is rolled, that is good luck. The next roll is multiplied by 2.

The list length will always be 3 or higher.

## Examples
```python
rolls([1, 2, 3]) ➞ 4
# The second roll, 2, counts as 0 as a result of rolling 1.

rolls([2, 6, 2, 5]) ➞ 17
# The 2 following the 6 was multiplied by 2.

rolls([6, 1, 1]) ➞ 8
# The first roll makes the second roll worth 2, but the
# second roll was still 1 so the third roll doesn't count.
```
## Notes

- Even if a 6 is rolled after a 1, 6 isn't summed but the 6's "effect" still takes place.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def rolls(dice: list[int]) -> int:
    return 0  # Put your code here!!!


test(662, rolls)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                6,
                1,
                1
            ]
        ],
        "return": 8
    },
    {
        "args": [
            [
                1,
                2,
                3
            ]
        ],
        "return": 4
    },
    {
        "args": [
            [
                6,
                6,
                6
            ]
        ],
        "return": 30
    },
    {
        "args": [
            [
                1,
                1,
                3,
                1,
                1
            ]
        ],
        "return": 2
    },
    {
        "args": [
            [
                1,
                1,
                1
            ]
        ],
        "return": 1
    }
]
```
## Credits

Found on Edabit: [Dice Gambling](https://edabit.com/challenge/Yfm3h3nT3apARd4gC)
