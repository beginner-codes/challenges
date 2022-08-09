# Challenge 514 - Snail Goes Up the Stairs

A snail goes up the stairs. Every step, he must go up the step, then go across to the next step. He wants to reach the top of the tower.

Write a function that returns the distance the snail must travel to the top of the tower given the height and length of each step and the height of the tower.

## Examples
```python
total_distance(0.2, 0.4, 100.0) ➞ 300.0
# Total distance is 300.

total_distance(0.3, 0.2, 25.0) ➞ 41.7

total_distance(0.1, 0.1, 6.0) ➞ 12.0
```
## Notes

- All given values are greater than `0`.
- Round answers to the nearest tenth `0.1`.
- Number of steps determined by tower height divided by stair height.
- For the purposes of this exercise, the last step's length must be counted to complete the journey.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def total_distance(step_height: float, step_width: float, tower_height: float) -> float:
    return 0.0 # Put your code here!!!


test(514, total_distance)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            0.2,
            0.1,
            100.6
        ],
        "return": 150.9
    },
    {
        "args": [
            1.0,
            1.0,
            777.0
        ],
        "return": 1554.0
    },
    {
        "args": [
            0.1,
            0.1,
            6.0
        ],
        "return": 12.0
    },
    {
        "args": [
            0.2,
            0.4,
            100.0
        ],
        "return": 300.0
    },
    {
        "args": [
            0.12,
            0.1,
            10.0
        ],
        "return": 18.3
    }
]
```
## Credits

Found on Edabit: [Snail Goes Up the Stairs](https://edabit.com/challenge/RxHMzNBx3HHNMydno)
