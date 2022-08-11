# Challenge 516 - Hall Monitor

A floor plan is arranged as follows:

- There are four rooms, which all lead into a hallway.
- It's impossible to move between rooms without first going into the hallway.

Create a function that validates whether the path between rooms is possible. The hallway will be given as the letter `"H"` and each room will be given as its room number.

## Examples
```python
possible_path([1, "H", 2, "H", 3, "H", 4]) ➞ True

possible_path(["H", 3, "H"]) ➞ True

possible_path([1, 2, "H", 3]) ➞ False
```
## Notes

- A route may begin or end in a hallway.
- All inputs are either numbers `1-4` or the letter `"H"`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def possible_path(path: list[int, str]) -> bool:
    return False # Put your code here!!!


test(516, possible_path)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                3,
                "H",
                2,
                "H",
                3,
                "H",
                1
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                3
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                "H",
                1,
                3
            ]
        ],
        "return": false
    },
    {
        "args": [
            [
                1,
                2,
                "H",
                3
            ]
        ],
        "return": false
    },
    {
        "args": [
            [
                "H",
                3,
                "H"
            ]
        ],
        "return": true
    }
]
```
## Credits

Found on Edabit: [Hall Monitor](https://edabit.com/challenge/G2QnBrxvpq9FacFuo)
