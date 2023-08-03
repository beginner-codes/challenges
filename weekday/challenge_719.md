# Challenge 719 - Fridge Poetry

Write a function that returns `True` if it's possible to build the second phrase using only the characters from the first phrase.

## Examples
```python
can_build("got 2 go", "gogogo 2 today") ➞ True

can_build("sit on top", "its a moo point") ➞ True

can_build("long high add or", "highway road go long") ➞ False

can_build("fill tuck mid", "truck falls dim") ➞ False
```
## Notes

- All letters will be in lower case.
- Numbers and special characters included.
- Ignore whitespaces.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def can_build(first: str, second: str) -> bool:
    return False  # Put your code here!!!


test(719, can_build)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "for an angel",
            "angel forest nymph awaken"
        ],
        "return": true
    },
    {
        "args": [
            "dool",
            "ken doll"
        ],
        "return": false
    },
    {
        "args": [
            "foolish prides",
            "foolish pride"
        ],
        "return": false
    },
    {
        "args": [
            "long high add or",
            "highway road go long"
        ],
        "return": false
    },
    {
        "args": [
            "world of make believe",
            "make believe world"
        ],
        "return": false
    }
]
```
## Credits

Found on Edabit: [Fridge Poetry](https://edabit.com/challenge/CD2fqbytBuXrbqJkL)
