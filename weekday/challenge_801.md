# Challenge 801 - Diagonal of a Cube

Create a function that takes the volume of a cube and returns the length of the cube's main diagonal, rounded to two decimal places.

## Examples
```python
cube_diagonal(8) ➞ 3.46

cube_diagonal(343) ➞ 12.12

cube_diagonal(1157.625) ➞ 18.19
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


def cube_diagonal(volume: int) -> float:
    return 0.0  # Put your code here!!!


test(801, cube_diagonal)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            48
        ],
        "return": 6.29
    },
    {
        "args": [
            343
        ],
        "return": 12.12
    },
    {
        "args": [
            1
        ],
        "return": 1.73
    },
    {
        "args": [
            1157.625
        ],
        "return": 18.19
    },
    {
        "args": [
            8
        ],
        "return": 3.46
    }
]
```

## Credits

Found on Edabit: [Diagonal of a Cube](https://edabit.com/challenge/9sN5tvXZjYCsKb4Mx)
