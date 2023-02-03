# Challenge 599 - Strange Pair

A pair of strings form a strange pair if both of the following are true:

- The 1st string's first letter = 2nd string's last letter.
- The 1st string's last letter = 2nd string's first letter.

Create a function that returns `True` if a pair of strings constitutes a strange pair, and `False` otherwise.

## Examples
```python
is_strange_pair("ratio", "orator") ➞ True
# "ratio" ends with "o" and "orator" starts with "o".
# "ratio" starts with "r" and "orator" ends with "r".

is_strange_pair("sparkling", "groups") ➞ True

is_strange_pair("bush", "hubris") ➞ False

is_strange_pair("", "") ➞ True
```
## Notes

- It should work on a pair of empty strings (they trivially share nothing).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def is_strange_pair(first_word: str, second_word: str) -> bool:
    return False  # Put your code here!!!


test(599, is_strange_pair)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "a",
            "b"
        ],
        "return": false
    },
    {
        "args": [
            "cupid",
            "dionysus"
        ],
        "return": false
    },
    {
        "args": [
            "&!",
            "!&"
        ],
        "return": true
    },
    {
        "args": [
            "False",
            "True"
        ],
        "return": false
    },
    {
        "args": [
            "futile",
            "elephant"
        ],
        "return": false
    }
]
```
## Credits

Found on Edabit: [Strange Pair](https://edabit.com/challenge/HWxNGdeoPxzievGa3)
