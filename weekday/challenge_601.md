# Challenge 601 - Grab the Numbers

Given a string including a bunch of characters and numbers, return the sum of all the numbers in the string. Note that multiple digits next to each other are counted as a whole number rather than separate digits.

## Examples
```python
grab_number_sum("aeiou250abc10") ➞ 260

grab_number_sum("one1two2twenty20") ➞ 23

grab_number_sum("900uwu50uwuuwuuwu25uwu25") ➞ 1000
```
## Notes

- Remember not to just add single digit numbers together, it should be possible for answers to easily get into the 100s!

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def grab_number_sum(string: str) -> int:
    return 0  # Put your code here!!!


test(601, grab_number_sum)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "75"
        ],
        "return": 75
    },
    {
        "args": [
            "one1two2twenty20"
        ],
        "return": 23
    },
    {
        "args": [
            "900uwu50uwuuwuuwu25uwu25"
        ],
        "return": 1000
    },
    {
        "args": [
            "aeiou5abc10"
        ],
        "return": 15
    },
    {
        "args": [
            "75shugeb15hvyff15"
        ],
        "return": 105
    }
]
```
## Credits

Found on Edabit: [Grab the Numbers](https://edabit.com/challenge/fvHLv9f5t6xoTWwXT)
