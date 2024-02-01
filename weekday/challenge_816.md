# Challenge 816 - Count the Points in a Circle

Count the total number of coordinates on a two-dimensional grid that are inside a given circle. The function has four parameters: the points (provided as a list of dictionaries), the circle's center x coordinate, the circle's center y coordinate, and the circle's radius.

## Examples
```python
points_in_circle([
  { "x": 0, "y": 0 },
  { "x": 1, "y": 1 },
  { "x": 0, "y": 5 },
  { "x": 10, "y": 10 }
], 0, 0, 5) ➞ 2
```
## Notes

- Only count the coordinates that are in the circle, not the ones that are on the border.

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


def points_in_circle(points: list[dict[str, int]], x: int, y: int, r: int) -> int:
    return 0  # Put your code here!!!


test(816, points_in_circle)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                {
                    "x": 0,
                    "y": 0
                },
                {
                    "x": 1,
                    "y": 1
                },
                {
                    "x": 0,
                    "y": 5
                },
                {
                    "x": 10,
                    "y": 10
                }
            ],
            50,
            50,
            40
        ],
        "return": 0
    },
    {
        "args": [
            [
                {
                    "x": 0,
                    "y": 0
                },
                {
                    "x": 1,
                    "y": 1
                },
                {
                    "x": 0,
                    "y": 5
                },
                {
                    "x": 10,
                    "y": 10
                }
            ],
            0,
            0,
            5
        ],
        "return": 2
    },
    {
        "args": [
            [
                {
                    "x": 8,
                    "y": 8
                },
                {
                    "x": 8,
                    "y": 6
                },
                {
                    "x": 4,
                    "y": 7
                }
            ],
            0,
            0,
            1
        ],
        "return": 0
    },
    {
        "args": [
            [
                {
                    "x": 10,
                    "y": 10
                },
                {
                    "x": 33,
                    "y": 54
                },
                {
                    "x": 7,
                    "y": 98
                },
                {
                    "x": 516,
                    "y": 85
                }
            ],
            23,
            94,
            100
        ],
        "return": 3
    },
    {
        "args": [
            [
                {
                    "x": 9,
                    "y": 6
                },
                {
                    "x": 9,
                    "y": 3
                },
                {
                    "x": 4,
                    "y": 8
                },
                {
                    "x": 3,
                    "y": 10
                },
                {
                    "x": 1,
                    "y": 6
                }
            ],
            0,
            0,
            7.5
        ],
        "return": 1
    }
]
```

## Credits

Found on Edabit: [Count the Points in a Circle](https://edabit.com/challenge/A9iPfSEZ9fCrPQSwC)
