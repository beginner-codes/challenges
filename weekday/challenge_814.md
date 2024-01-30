# Challenge 814 - Solving Linear Equations

Consider the equation `ax+1=b+x` where `a` and `b` are constants. Create a function that takes numbers `a` and `b` as arguments, and returns the solution of the equation.

- If the equation does not have a solution, return `"No solution"`.
- If any number satisfies the equation, return `"Any number"`.

## Examples
```python
solve(4, 7) ➞ 2.0

solve(9, 5) ➞ 0.5

solve(12, -4) ➞ -0.455
```
## Notes

- Round your answer to three decimal places.

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


def solve(a: int, b: int) -> float:
    return 0.0  # Put your code here!!!


test(814, solve)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            100,
            7
        ],
        "return": 0.061
    },
    {
        "args": [
            9,
            5
        ],
        "return": 0.5
    },
    {
        "args": [
            4,
            7
        ],
        "return": 2.0
    },
    {
        "args": [
            1,
            1
        ],
        "return": "Any number"
    },
    {
        "args": [
            1,
            2
        ],
        "return": "No solution"
    }
]
```

## Credits

Found on Edabit: [Solving Linear Equations (Part 1)](https://edabit.com/challenge/wW2z9bRi2bTeAbcqY)
