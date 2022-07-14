# Challenge 478 - A Letter's Best Friend

Given a string, return if a given letter always appears immediately before another given letter.

## Worked Example
```python
best_friend("he headed to the store", "h", "e") ➞ True

# All occurences of "h": ["he", "headed", "the"]
# All occurences of "h" have an "e" after it.
# Return True
```
## Examples
```python
best_friend("he headed to the store", "h", "e") ➞ True

best_friend("i found an ounce with my hound", "o", "u") ➞ True

best_friend("we found your dynamite", "d", "y") ➞ False
```
## Notes

- Don't count letters with spaces between them.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def best_friend(string: str, first_letter: str, second_letter: str) -> bool:
    return False  # Put your code here!!!


test(478, best_friend)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "he headed to the store",
            "h",
            "e"
        ],
        "return": true
    },
    {
        "args": [
            "i found an ounce with my hound",
            "o",
            "u"
        ],
        "return": true
    },
    {
        "args": [
            "those were their thorns they said",
            "t",
            "h"
        ],
        "return": true
    },
    {
        "args": [
            "we found your dynamite",
            "d",
            "y"
        ],
        "return": false
    },
    {
        "args": [
            "look they took the cookies",
            "o",
            "o"
        ],
        "return": false
    },
    {
        "args": [
            "go to edabit and meditate",
            "e",
            "d"
        ],
        "return": false
    }
]
```
## Credits

Found on Edabit: [A Letter's Best Friend](https://edabit.com/challenge/59kkN3yDnFKHYfgMm)
