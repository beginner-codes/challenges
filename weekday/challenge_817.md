# Challenge 817 - Algebra Sequence — Boxes

Create a function that takes a number (step) as an argument and returns the amount of boxes in that step of the sequence.

Use this algorithm:
- Step 0: Start with 0
- Step 1: Add 3
- Step 2: Subtract 1
- Repeat Step 1 & 2

Here's a visual representation:
```
Step 1     Step 2     Step 3
 □ □        □ □        □ □
 □                     □ □
                       □
                             
Step 4     Step 5     Step 6
 □ □        □ □        □ □
 □ □        □ □        □ □
            □ □        □ □
            □

```

## Examples
```python
box_seq(0) ➞ 0

box_seq(1) ➞ 3

box_seq(2) ➞ 2
```

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


def box_step(step: int) -> int:
    return 0  # Put your code here!!!


test(817, box_step)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            0
        ],
        "return": 0
    },
    {
        "args": [
            1
        ],
        "return": 3
    },
    {
        "args": [
            99
        ],
        "return": 101
    },
    {
        "args": [
            5
        ],
        "return": 7
    },
    {
        "args": [
            2
        ],
        "return": 2
    },
    {
        "args": [
            6
        ],
        "return": 6
    }
]
```

## Credits

Found on Edabit: [Algebra Sequence — Boxes](https://edabit.com/challenge/baBNZFCozmjNhbp9Q)
