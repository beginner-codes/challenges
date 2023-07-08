# Challenge 701 - Widen the Streets!

Given a list of strings depicting a row of buildings, create a function which sets the gap between buildings to a given amount.

## Examples
```python
widen_streets([
  "###   ## #",
  "### # ## #",
  "### # ## #",
  "### # ## #",
  "### # ## #"
], 3) ➞
[
  "###       ##   #",
  "###   #   ##   #",
  "###   #   ##   #",
  "###   #   ##   #",
  "###   #   ##   #"
]

widen_streets([
  "## ### ###",
  "## ### ###",
  "## ### ###",
  "## ### ###"
], 2) ➞
[
  "##  ###  ###",
  "##  ###  ###",
  "##  ###  ###",
  "##  ###  ###"
]

widen_streets([
  "# # # # #"
], 2) ➞
[
  "#  #  #  #  #"
]
```
## Notes

- Buildings may be different sizes.
- There will always be a starting gap size of one character.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def widen_streets(buildings: list[str], width: int) -> list[str]:
    return []  # Put your code here!!!


test(701, widen_streets)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "###   ## #",
                "### # ## #",
                "### # ## #",
                "### # ## #",
                "### # ## #"
            ],
            3
        ],
        "return": [
            "###       ##   #",
            "###   #   ##   #",
            "###   #   ##   #",
            "###   #   ##   #",
            "###   #   ##   #"
        ]
    },
    {
        "args": [
            [
                "# # # # #"
            ],
            2
        ],
        "return": [
            "#  #  #  #  #"
        ]
    },
    {
        "args": [
            [
                "## ### ###",
                "## ### ###",
                "## ### ###",
                "## ### ###"
            ],
            2
        ],
        "return": [
            "##  ###  ###",
            "##  ###  ###",
            "##  ###  ###",
            "##  ###  ###"
        ]
    }
]
```
## Credits

Found on Edabit: [Widen the Streets!](https://edabit.com/challenge/k87ztfzqrpPHvgNWR)
