# Challenge 795 - Tower of Hanoi

There are three towers. The objective of the game is to move all the disks over to tower #3, but you can't place a larger disk onto a smaller disk.

Create a function that takes a number of discs as an argument and returns the minimum number of steps needed to complete the game.

## Examples
```python
tower_hanoi(3) ➞ 7

tower_hanoi(5) ➞ 31

tower_hanoi(0) ➞ 0
```
## Notes

- The amount of discs is always a positive integer.
- 1 disc can be changed per move.

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


def tower_hanoi(discks: int) -> int:
    return 0  # Put your code here!!!


test(795, tower_hanoi)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            13
        ],
        "return": 8191
    },
    {
        "args": [
            0
        ],
        "return": 0
    },
    {
        "args": [
            8
        ],
        "return": 255
    },
    {
        "args": [
            19
        ],
        "return": 524287
    },
    {
        "args": [
            5
        ],
        "return": 31
    }
]
```

## Credits

Found on Edabit: [Tower of Hanoi](https://edabit.com/challenge/ZmjLLhFc4TqaMPSki)
