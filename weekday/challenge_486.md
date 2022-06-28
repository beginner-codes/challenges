# Challenge 486 - Remove Duplicates from a List

Create a function that takes a list of items, removes all duplicate items and returns a new list in the same sequential order as the old list (minus duplicates).

## Examples
```python
remove_dups([1, 0, 1, 0]) ➞ [1, 0]

remove_dups(["The", "big", "cat"]) ➞ ["The", "big", "cat"]

remove_dups(["John", "Taylor", "John"]) ➞ ["John", "Taylor"]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test
from typing import TypeVar

T = TypeVar("T")

def remove_dups(items: list[T]) -> list[T]:
    return []  # Put your code here!!!


test(486, remove_dups)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "John",
                "Taylor",
                "John"
            ]
        ],
        "return": [
            "John",
            "Taylor"
        ]
    },
    {
        "args": [
            [
                "John",
                "Taylor",
                "John",
                "john"
            ]
        ],
        "return": [
            "John",
            "Taylor",
            "john"
        ]
    },
    {
        "args": [
            [
                "javascript",
                "python",
                "python",
                "ruby",
                "javascript",
                "c",
                "ruby"
            ]
        ],
        "return": [
            "javascript",
            "python",
            "ruby",
            "c"
        ]
    },
    {
        "args": [
            [
                1,
                2,
                2,
                2,
                3,
                2,
                5,
                2,
                6,
                6,
                3,
                7,
                1,
                2,
                5
            ]
        ],
        "return": [
            1,
            2,
            3,
            5,
            6,
            7
        ]
    },
    {
        "args": [
            [
                "#",
                "#",
                "%",
                "&",
                "#",
                "$",
                "&"
            ]
        ],
        "return": [
            "#",
            "%",
            "&",
            "$"
        ]
    },
    {
        "args": [
            [
                3,
                "Apple",
                3,
                "Orange",
                "Apple"
            ]
        ],
        "return": [
            3,
            "Apple",
            "Orange"
        ]
    }
]
```
## Credits

Found on Edabit: [Remove Duplicates from a List](https://edabit.com/challenge/SLCqbNTy4aacoNjvw)
