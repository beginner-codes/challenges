# Challenge 561 - Christmas Tree

Write a function to create a Christmas tree of a given height.

## Examples
```python
tree(1) ➞ [
  "#"
]

tree(2) ➞ [
  " # ",
  "###"
]

tree(5) ➞ [
  "    #    ",
  "   ###   ",
  "  #####  ",
  " ####### ",
  "#########"
]

tree(0) ➞ []
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def tree(height: int) -> list[str]:
    return [] # Put your code here!!!


test(561, tree)  # Tell it which challenge to test against
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
            2
        ],
        "return": [
            " # ",
            "###"
        ]
    },
    {
        "args": [
            5
        ],
        "return": [
            "    #    ",
            "   ###   ",
            "  #####  ",
            " ####### ",
            "#########"
        ]
    },
    {
        "args": [
            0
        ],
        "return": []
    }
]
```
## Credits

Found on Edabit: [Christmas Tree](https://edabit.com/challenge/vYYfFAAfjoc8crCqu)
