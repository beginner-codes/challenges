# Challenge 515 - Replacing Letters with Hashes

Write a function that replaces all letters within a given range with the hash symbol `#`.

## Examples
```python
replace("abcdef", "c-e") ➞ "ab###f"

replace("rattle", "r-z") ➞ "#a##le"

replace("microscopic", "i-i") ➞ "m#croscop#c"

replace("", "a-z") ➞ ""
```
## Notes

- The range will always be in order, a.k.a. for `m-n`, character `m` will always come before or equal `n`.
- Strings will be in lower case letters only.
- Return an empty string if the input is an empty string.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def replace(string: str, letter_range: str) -> str:
    return "" # Put your code here!!!


test(515, replace)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "",
            "a-z"
        ],
        "return": ""
    },
    {
        "args": [
            "abcdef",
            "c-e"
        ],
        "return": "ab###f"
    },
    {
        "args": [
            "bountiful",
            "a-o"
        ],
        "return": "##u#t##u#"
    },
    {
        "args": [
            "rattle",
            "r-z"
        ],
        "return": "#a##le"
    },
    {
        "args": [
            "microscopic",
            "i-i"
        ],
        "return": "m#croscop#c"
    }
]
```
## Credits

Found on Edabit: [Replacing Letters with Hashes](https://edabit.com/challenge/6pjjWy5ST2eMKtGkh)
