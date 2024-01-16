# Challenge 804 - String Pairs

Create a function that takes a string and returns a list of two-paired characters. If the string has an odd number of characters, add an asterisk `*` in the final pair.

## Examples
```python
string_pairs("airforces") ➞ ["ai", "rf", "or", "ce", "s*"]

string_pairs("abcdef") ➞ ["ab", "cd", "ef"] 

string_pairs("red") ➞ ["re", "d*"]
```
## Notes

- Return `[]` if the given string is empty.

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


def string_pairs(string: str) -> list[str]:
    return []  # Put your code here!!!


test(804, string_pairs)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            "airforces"
        ],
        "return": [
            "ai",
            "rf",
            "or",
            "ce",
            "s*"
        ]
    },
    {
        "args": [
            ""
        ],
        "return": []
    },
    {
        "args": [
            "abcdef"
        ],
        "return": [
            "ab",
            "cd",
            "ef"
        ]
    },
    {
        "args": [
            "beginnercodes"
        ],
        "return": [
            "be",
            "gi",
            "nn",
            "er",
            "co",
            "de",
            "s*"
        ]
    },
    {
        "args": [
            "pak"
        ],
        "return": [
            "pa",
            "k*"
        ]
    }
]
```

## Credits

Found on Edabit: [String Pairs](https://edabit.com/challenge/ZDSrKXGH4dG9M4iuP)
