# Challenge 718 - First Before Second Letter

You are given three inputs: a string, one letter, and a second letter.

Write a function that returns `True` if every instance of the first letter occurs before every instance of the second letter.

## Examples
```python
first_before_second("a rabbit jumps joyfully", "a", "j") ➞ True
# Every instance of "a" occurs before every instance of "j".

first_before_second("knaves knew about waterfalls", "k", "w") ➞  True

first_before_second("happy birthday", "a", "y") ➞ False
# The "a" in "birthday" occurs after the "y" in "happy".

first_before_second("precarious kangaroos", "k", "a") ➞ False
```
## Notes

- All strings will be in lower case.
- All strings will contain the first and second letters at least once.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def first_before_second(string: str, a: str, b: str) -> bool:
    return False  # Put your code here!!!


test(718, first_before_second)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "the hostess made pecan pie",
            "h",
            "p"
        ],
        "return": true
    },
    {
        "args": [
            "barry the butterfly flew away",
            "b",
            "f"
        ],
        "return": true
    },
    {
        "args": [
            "maria makes money",
            "m",
            "o"
        ],
        "return": true
    },
    {
        "args": [
            "moody muggles",
            "m",
            "o"
        ],
        "return": false
    },
    {
        "args": [
            "sharp cheddar biscuit",
            "t",
            "s"
        ],
        "return": false
    }
]
```
## Credits

Found on Edabit: [First Before Second Letter](https://edabit.com/challenge/D6XfxhRobdQvbKX4v)
