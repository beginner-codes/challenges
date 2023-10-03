# Challenge 763 - Perimeters

Write a function that takes a number and returns the perimeter of either a circle or a square. The input will be in the form `(letter, number)` where the letter will be either `"s"` for square, or `"c"` for circle, and the number will be the side of the square or the radius of the circle.

Use the following formulas:

- Perimeter of a square: 4 * side.
- Perimeter of a circle: 6.28 * radius.

## Examples
```python
perimeter("s", 7) ➞ 28

perimeter("c", 4) ➞ 25.12

perimeter("c", 9) ➞ 56.52
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
from typing import Literal
from beginnercodes.challenges import test


def perimeter(shape: Literal["c"] | Literal["s"], size: int) -> float:
    return 0.0  # Put your code here!!!


test(763, perimeter)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            "s",
            13
        ],
        "return": 52
    },
    {
        "args": [
            "s",
            1
        ],
        "return": 4
    },
    {
        "args": [
            "s",
            30
        ],
        "return": 120
    },
    {
        "args": [
            "c",
            4
        ],
        "return": 25.12
    },
    {
        "args": [
            "c",
            1
        ],
        "return": 6.28
    },
    {
        "args": [
            "c",
            13
        ],
        "return": 81.64
    }
]
```

## Credits

Found on Edabit: [Perimeters with a Catch](https://edabit.com/challenge/zkKNmC66ASvSm5wJA)
