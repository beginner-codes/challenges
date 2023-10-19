# Challenge 775 - A Simple Equation

Create a function which takes three numbers: a, b and c, and returns a list of equations as strings using simple arithmetic operators (+, -, *, /).

Return each valid equation using the given values.

## Examples
```python
simple_equation(1, 2, 3) ➞ ["1+2=3", "2+1=3", "3-1=2", "3-2=1"]

simple_equation(2, 2, 4) ➞ ["2*2=4", "2+2=4", "4-2=2", "4/2=2"]

simple_equation(6, 2, 3) ➞ ["2*3=6", "3*2=6", "6/2=3", "6/3=2"]
```
## Notes

- If no solutions are possible return an empty list
- Sort the solution strings in ascending order 

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


def simple_equation(a: int, b: int, c: int) -> list[str]:
    return []  # Put your code here!!!


test(775, simple_equation)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            2,
            2,
            4
        ],
        "return": [
            "2*2=4",
            "2+2=4",
            "4-2=2",
            "4/2=2"
        ]
    },
    {
        "args": [
            6,
            2,
            3
        ],
        "return": [
            "2*3=6",
            "3*2=6",
            "6/2=3",
            "6/3=2"
        ]
    },
    {
        "args": [
            1,
            2,
            3
        ],
        "return": [
            "1+2=3",
            "2+1=3",
            "3-1=2",
            "3-2=1"
        ]
    },
    {
        "args": [
            6,
            5,
            4
        ],
        "return": []
    },
    {
        "args": [
            2,
            3,
            4
        ],
        "return": []
    }
]
```

## Credits

Found on Edabit: [A Simple Equation](https://edabit.com/challenge/mYGipMffRTYxYmv5i)
