# Challenge 654 - Number of Paths Between Points

This challenge deals with finding and counting the number of paths between points on a rectilinear grid. A starting point `(x, y)` with non-negative integer coordinates is provided. You are only allowed to move horizontally and vertically along the grid. Hence, from `(x, y)` you may move to `(x+1, y)`, `(x-1, y)`, `(x, y+1)`, or `(x, y-1)`. Your goal is to return to the origin `(0, 0)` in such a way that you never increase the distance to the origin. The distance is counted as the minimum number of total vertical and horizontal steps to reach the origin.

Create a function that reads a starting location, `(x, y)` and returns the total number of different paths back to the origin. Two paths are different if there is at least one step on the path that is different even if most of the steps are the same.

## Examples
```python
paths(0, 0) ➞ 1

paths(2, 1) ➞ 3

paths(2, 2) ➞ 6
```
## Notes

- The return type for this function is a positive integer.
- `x` and `y` will always be integers greater than or equal to `0`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def paths(x: int, y: int) -> int:
    return 0  # Put your code here!!!


test(654, paths)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            6,
            9
        ],
        "return": 5005
    },
    {
        "args": [
            2,
            1
        ],
        "return": 3
    },
    {
        "args": [
            7,
            0
        ],
        "return": 1
    },
    {
        "args": [
            0,
            0
        ],
        "return": 1
    },
    {
        "args": [
            1,
            99
        ],
        "return": 100
    }
]
```
## Credits

Found on Edabit: [Number of Paths Between Points](https://edabit.com/challenge/hpgTmtkEiKfm5xxGy)
