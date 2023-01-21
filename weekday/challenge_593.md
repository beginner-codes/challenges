# Challenge 593 - Sherlock and the Valid String

Sherlock considers a string to be valid if all characters of the string appear the same number of times. It is also valid if he can remove just 1 character at 1 index in the string, and the remaining characters will occur the same number of times. Given a string, determine if it is valid. If so, return `"YES"`, otherwise return `"NO"`.

For example, `"abc"`, the string is valid because the frequencies of characters are all the same. For `"abcc"`, the string is also valid, because we can remove 1 `"c"` and have one of each character remaining in the string. However, `"abccc"`, the string is not valid, because removing one character does not result in the same frequency of characters.

## Examples
```python
is_valid("aabbcd") ➞ "NO"
# We would need to remove two characters, both c and d  -> aabb or a and b -> abcd, to make it valid.
# We are limited to removing only one character, so it is invalid.

is_valid("aabbccddeefghi") ➞ "NO"
# Frequency counts for the letters are as follows:
# {"a": 2, "b": 2, "c": 2, "d": 2, "e": 2, "f": 1, "g": 1, "h": 1, "i": 1}
# There are two ways to make the valid string:
# Remove 4 characters with a frequency of 1: {f, g, h, i}.
# Remove 5 characters of frequency 2: {a, b, c, d, e}.
# Neither of these is an option.

is_valid("abcdefghhgfedecba") ➞ "YES"
# All characters occur twice except for e which occurs 3 times.
# We can delete one instance of e to have a valid string.
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def is_valid(text: str) -> str:
    return ""  # Put your code here!!!


test(593, is_valid)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "aabbcd"
        ],
        "return": "NO"
    },
    {
        "args": [
            "abcc"
        ],
        "return": "YES"
    },
    {
        "args": [
            "abccc"
        ],
        "return": "NO"
    },
    {
        "args": [
            "abcdefghhgfedecba"
        ],
        "return": "YES"
    },
    {
        "args": [
            "aabbccddeefghi"
        ],
        "return": "NO"
    }
]
```
## Credits

Found on Edabit: [Sherlock and the Valid String](https://edabit.com/challenge/738WMYrYWPXeBgzFs)
