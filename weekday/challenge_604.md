# Challenge 604 - String Incrementer

Write a function which increments a string to create a new string.

- If the string ends with a number, the number should be incremented by `1`.
- If the string doesn't end with a number, `1` should be added to the new string.
- If the number has leading zeros, the amount of digits should be considered.

## Examples
```python
increment_string("foo") ➞ "foo1"

increment_string("foobar0009") ➞ "foobar0010"

increment_string("foo099") ➞ "foo100"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def increment_string(string: str) -> str:
    return ""  # Put your code here!!!


test(604, increment_string)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "foo"
        ],
        "return": "foo1"
    },
    {
        "args": [
            "foobar00599"
        ],
        "return": "foobar00600"
    },
    {
        "args": [
            "foo09999"
        ],
        "return": "foo10000"
    },
    {
        "args": [
            "foo099"
        ],
        "return": "foo100"
    },
    {
        "args": [
            "foobar01002"
        ],
        "return": "foobar01003"
    }
]
```
## Credits

Found on Edabit: [String Incrementer](https://edabit.com/challenge/Rn3g3hokznLu8ZtDP)
