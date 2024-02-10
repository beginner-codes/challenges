# Challenge 822 - Is This a Right Angled Triangle?

Given three numbers, determine whether they are the edges of a right-angled triangle.

## Examples
```python
right_triangle(3, 4, 5) ➞ True
# This is the classic example of a "nice" right angled triangle.

right_triangle(145, 105, 100) ➞ True
# This is a less famous example.

right_triangle(70, 130, 110) ➞ False
# This isn't a right angled triangle.
```
## Notes

- Notice the largest side of the triangle might not be the last one passed to the function
- All numbers will be integers

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


def right_triangle(x: int, y: int, z: int) -> bool:
    return False  # Put your code here!!!


test(822, right_triangle)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            915,
            1748,
            1973
        ],
        "return": true
    },
    {
        "args": [
            0,
            4,
            4
        ],
        "return": false
    },
    {
        "args": [
            70,
            130,
            110
        ],
        "return": false
    },
    {
        "args": [
            140,
            170,
            220
        ],
        "return": false
    },
    {
        "args": [
            60,
            60,
            60
        ],
        "return": false
    }
]
```

## Credits

Found on Edabit: [Is This a Right Angled Triangle?](https://edabit.com/challenge/mPpcATtDMYiegZ3Jw)
