# Challenge 551 - Making a Simple Dartboard

Create a function which creates a square dartboard with a given side length. The value of a number should increase the closer it is to the center of the board.

## Examples
```python
make_dartboard(3) ➞ [
  111,
  121,
  111
]

make_dartboard(8) ➞ [
  11111111,
  12222221,
  12333321,
  12344321,
  12344321,
  12333321,
  12222221,
  11111111
]

make_dartboard(5) ➞ [
  11111,
  12221,
  12321,
  12221,
  11111
]
```
## Notes

- If the size given is an even number, the center should be made up of the 4 highest values.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def make_dartboard(size: int) -> list[int]:
    return [] # Put your code here!!!


test(551, make_dartboard)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            6
        ],
        "return": [
            111111,
            122221,
            123321,
            123321,
            122221,
            111111
        ]
    },
    {
        "args": [
            5
        ],
        "return": [
            11111,
            12221,
            12321,
            12221,
            11111
        ]
    },
    {
        "args": [
            7
        ],
        "return": [
            1111111,
            1222221,
            1233321,
            1234321,
            1233321,
            1222221,
            1111111
        ]
    },
    {
        "args": [
            2
        ],
        "return": [
            11,
            11
        ]
    },
    {
        "args": [
            4
        ],
        "return": [
            1111,
            1221,
            1221,
            1111
        ]
    }
]
```
## Credits

Found on Edabit: [Making a Simple Dartboard](https://edabit.com/challenge/Kv8DMmwfuKTLyZD5E)
