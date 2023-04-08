# Challenge 640 - Mountains or Valleys

A mountain is a list with exactly one peak.

- All numbers to the left of the peak are increasing.
- All numbers to the right of the peak are decreasing.
- The peak CANNOT be on the boundary.

A valley is a list with exactly one trough.

- All numbers to the left of the trough are decreasing.
- All numbers to the right of the trough are increasing.
- The trough CANNOT be on the boundary. 

Some examples of mountains and valleys:
```python
Mountain A:  [1, 3, 5, 4, 3, 2]   # 5 is the peak
Mountain B:  [-1, 0, -1]   # 0 is the peak
Mountain B:  [-1, -1, 0, -1, -1]   # 0 is the peak (plateau on both sides is okay)

Valley A: [10, 9, 8, 7, 2, 3, 4, 5]   # 2 is the trough
Valley B: [350, 100, 200, 400, 700]  # 100 is the trough
```
Neither mountains nor valleys:
```python
Landscape A: [1, 2, 3, 2, 4, 1]  # 2 peaks (3, 4), not 1
Landscape B: [5, 4, 3, 2, 1]  # Peak cannot be a boundary element
Landscape B: [0, -1, -1, 0, -1, -1]  # 2 peaks (0)
```
Based on the rules above, write a function that takes in a list and returns either `"mountain"`, `"valley"`, or `"neither"`.

## Examples
```python
landscape_type([3, 4, 5, 4, 3]) ➞ "mountain"

landscape_type([9, 7, 3, 1, 2, 4]) ➞ "valley"

landscape_type([9, 8, 9]) ➞ "valley"

landscape_type([9, 8, 9, 8]) ➞ "neither"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def landscape_type(land: list[int]) -> str:
    return ""  # Put your code here!!!


test(640, landscape_type)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                1,
                2,
                3,
                4
            ]
        ],
        "return": "neither"
    },
    {
        "args": [
            [
                9,
                8,
                9
            ]
        ],
        "return": "valley"
    },
    {
        "args": [
            [
                9,
                7,
                3,
                1,
                2,
                4
            ]
        ],
        "return": "valley"
    },
    {
        "args": [
            [
                9,
                8,
                9,
                8
            ]
        ],
        "return": "neither"
    },
    {
        "args": [
            [
                0,
                -1,
                -1,
                0,
                -1,
                -1
            ]
        ],
        "return": "neither"
    }
]
```
## Credits

Found on Edabit: [Mountains or Valleys](https://edabit.com/challenge/5h5uAmaAWY3jSHA7k)
