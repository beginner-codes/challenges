# Challenge 573 - Directionally Challenged

Suppose you are directionally challenged, and get lost easily. As a result, sometimes you walk in circles or make U-turns. You might take a suboptimal route. Create a function that returns the difference in length between your path and the optimal path. Both paths reach the same destination.

You start at `(0,0)` and reach your destination by the end of the input list.

A demonstration:
```python
Your route: ["N", "S", "E", "W", "E", "E", "E", "N"]  // 8
Optimal route: ["E", "E", "E", "N"] (or ["N", "E", "E", "E"], etc.) // 4
# Difference in length: 8 - 4 = 4

# Explanation: Your "S" cancels out your "N" and your "W" cancels out your "E" leaving you back at (0,0)
```
## Examples
```python
route_diff(["N", "E", "S", "W"]) ➞ 4
# You"ve just walked in a circle! You are back at the origin. Your optimal path was `[]`.

route_diff(["N", "N", "N", "E", "N", "E"]) ➞ 0
# No improvements here!

route_diff(["N", "S", "N", "S", "E", "W", "E", "E"]) ➞ 6
```
## Notes

- Remember that an `N` cancels out an `S`, and an `E` cancels out a `W`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def route_diff(path: list[str]) -> int:
    return int  # Put your code here!!!


test(573, route_diff)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "N",
                "N",
                "S",
                "S",
                "S",
                "S",
                "E"
            ]
        ],
        "return": 4
    },
    {
        "args": [
            [
                "N",
                "E",
                "S",
                "W"
            ]
        ],
        "return": 4
    },
    {
        "args": [
            [
                "N",
                "S",
                "N",
                "S",
                "E",
                "W",
                "E",
                "E"
            ]
        ],
        "return": 6
    },
    {
        "args": [
            [
                "N",
                "S",
                "N",
                "S",
                "E"
            ]
        ],
        "return": 4
    },
    {
        "args": [
            [
                "S",
                "S",
                "S"
            ]
        ],
        "return": 0
    }
]
```
## Credits

Found on Edabit: [Directionally Challenged](https://edabit.com/challenge/bHfb35MfsjyM6DJge)
