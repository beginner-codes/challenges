# Challenge 565 - Neighboring Letters

Create a function that takes a string and checks if every single character is preceded and followed by a character adjacent to it in the english alphabet.

Example: `"b"` should be preceded and followed by ether `"a"` or `"c"` (`abc` or `cba` or `aba` or `cbc` == `True` but `abf` or `zbc` == `False`).

## Examples
```python
neighboring("aba") ➞ True

neighboring("abcdedcba") ➞ True

neighboring("efghihfe") ➞ False

neighboring("abc") ➞ True

neighboring("qrstuv") ➞ True

neighboring("mnopqrstsrqponm") ➞ True
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def neighboring(lettetrs: str) -> bool:
    return False # Put your code here!!!


test(565, neighboring)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "aaaaa"
        ],
        "return": false
    },
    {
        "args": [
            "xyzyx"
        ],
        "return": true
    },
    {
        "args": [
            "zyz"
        ],
        "return": true
    },
    {
        "args": [
            "qrstuv"
        ],
        "return": true
    },
    {
        "args": [
            "mnopqrstsrqponm"
        ],
        "return": true
    },
    {
        "args": [
            "cdefg"
        ],
        "return": true
    },
    {
        "args": [
            "aba"
        ],
        "return": true
    },
    {
        "args": [
            "efghihfe"
        ],
        "return": false
    },
    {
        "args": [
            "aeiou"
        ],
        "return": false
    },
    {
        "args": [
            "abcdedcba"
        ],
        "return": true
    }
]
```
## Credits

Found on Edabit: [Neighboring Letters](https://edabit.com/challenge/oK2e5Xet35ZFZNLX6)
