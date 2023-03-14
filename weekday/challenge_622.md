# Challenge 622 - Calculate the Shortest Distance Between Two Points

Create a function that takes a string of four numbers. These numbers represent two separate points on a graph known as the x-axis (horizontal axis) and y-axis (vertical axis).

The order of coordinates in the string corresponds as follows:
```python
"x1,y1,x2,y2"
```
Calculate the distance between `x` and `y`.

## Examples
```python
shortest_distance("1,1,2,1") ➞ 1

shortest_distance("1,1,3,1") ➞ 2

shortest_distance("-5,1,3,1") ➞ 8

shortest_distance("-5,2,3,1") ➞ 8.06
```
## Notes

- All floats fixed to two decimal places (e.g. `2.34`).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def shortest_distance(coordinates: str) -> float:
    return 0.0  # Put your code here!!!


test(622, shortest_distance)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "93640,215647,905863,676918"
        ],
        "return": 934064.85
    },
    {
        "args": [
            "183757,435586,10021,236721"
        ],
        "return": 264067.2
    },
    {
        "args": [
            "124164,251582,528462,653536"
        ],
        "return": 570108.67
    },
    {
        "args": [
            "388776,95216,206886,917821"
        ],
        "return": 842474.31
    },
    {
        "args": [
            "282910,113617,745331,249114"
        ],
        "return": 481863.69
    }
]
```
## Credits

Found on Edabit: [Calculate the Shortest Distance Between Two Points](https://edabit.com/challenge/HvsBiHLGcsv2ex3gv)
