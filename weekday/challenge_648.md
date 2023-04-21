# Challenge 648 - Making a Box

Create a function that generates a box of the given size.

## Examples
```python
make_box(5) ➞ [
  "#####",
  "#   #",
  "#   #",
  "#   #",
  "#####"
]

make_box(3) ➞ [
  "###",
  "# #",
  "###"
]

make_box(2) ➞ [
  "##",
  "##"
]

make_box(1) ➞ [
  "#"
]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def make_box(size: int) -> list[str]:
    return []  # Put your code here!!!


test(648, make_box)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            1
        ],
        "return": [
            "#"
        ]
    },
    {
        "args": [
            6
        ],
        "return": [
            "######",
            "#    #",
            "#    #",
            "#    #",
            "#    #",
            "######"
        ]
    },
    {
        "args": [
            4
        ],
        "return": [
            "####",
            "#  #",
            "#  #",
            "####"
        ]
    },
    {
        "args": [
            2
        ],
        "return": [
            "##",
            "##"
        ]
    },
    {
        "args": [
            5
        ],
        "return": [
            "#####",
            "#   #",
            "#   #",
            "#   #",
            "#####"
        ]
    }
]
```
## Credits

Found on Edabit: [Making a Box](https://edabit.com/challenge/dy3WWJr34gSGRPLee)
