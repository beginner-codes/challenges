# Challenge 758 - Sort by the Letters

Write a function that sorts each string in a list by the letter in alphabetic ascending order (a-z).

## Examples
```python
sort_by_letter(["932c", "832u32", "2344b"])
➞ ["2344b", "932c", "832u32"]

sort_by_letter(["99a", "78b", "c2345", "11d"])
➞ ["99a", "78b", "c2345", "11d"]

sort_by_letter(["572z", "5y5", "304q2"])
➞ ["304q2", "5y5", "572z"]

sort_by_letter([])
➞ []
```
## Notes

- Each string will only have one (lowercase) letter.
- If given an empty list, return an empty list.

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


def sort_by_letter(strings: list[str]) -> list[str]:
    return []  # Put your code here!!!


test(758, sort_by_letter)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                "99a",
                "78b",
                "c2345",
                "11d"
            ]
        ],
        "return": [
            "99a",
            "78b",
            "c2345",
            "11d"
        ]
    },
    {
        "args": [
            [
                "572z",
                "5y5",
                "304q2"
            ]
        ],
        "return": [
            "304q2",
            "5y5",
            "572z"
        ]
    },
    {
        "args": [
            []
        ],
        "return": []
    },
    {
        "args": [
            [
                "932c",
                "832u32",
                "2344b"
            ]
        ],
        "return": [
            "2344b",
            "932c",
            "832u32"
        ]
    }
]
```

## Credits

Found on Edabit: [Sort by the Letters](https://edabit.com/challenge/LhMkMu46rG8EweYf7)
