# Challenge 744 - Is the Input Factorial of an Integer?

Create a function that checks if a given integer is exactly the factorial of an integer or not. `True` if it is, `False` otherwise.

## Examples
```python
is_factorial(2) ➞ True
# 2 = 2 * 1 = 2!

is_factorial(27) ➞ False

is_factorial(24) ➞ True
# 24 = 4 * 3 * 2 * 1 = 4!
```
## Notes

- No error handling is necessary. Inputs are all positive integers.
- Alternatively, you can solve this with a recursive approach.

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


def is_factorial(num: int) -> bool:
    return False  # Put your code here!!!


test(744, is_factorial)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            24
        ],
        "return": true
    },
    {
        "args": [
            721
        ],
        "return": false
    },
    {
        "args": [
            6
        ],
        "return": true
    },
    {
        "args": [
            16
        ],
        "return": false
    },
    {
        "args": [
            36
        ],
        "return": false
    }
]
```

## Credits

Found on Edabit: [Is the Input Factorial of an Integer?](https://edabit.com/challenge/ozMMLxJRPXBwm3yTP)
