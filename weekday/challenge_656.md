# Challenge 656 - Flick Switch

Create a function that always returns `True` for every item in a given list. However, if an element is the word `"flick"`, switch to always returning the opposite boolean value.

## Examples
```python
flick_switch(["beginner.codes", "flick", "beginner", "codes"]) ➞ [True, False, False, False]

flick_switch(["flick", 11037, 3.14, 53]) ➞[False, False, False, False]

flick_switch([False, False, "flick", "sheep", "flick"]) ➞ [True, True, False, False, True]
```
## Notes

- `"flick"` will always be given in lowercase.
- A list may contain multiple flicks.
- Switch the boolean value on the same element as the flick itself.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from typing import Any
from beginnercodes.challenges import test


def flick_switch(values: list[Any]) -> list[bool]:
    return []  # Put your code here!!!


test(656, flick_switch)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "beginner.codes",
                "flick",
                "beginner",
                "codes"
            ]
        ],
        "return": [
            true,
            false,
            false,
            false
        ]
    },
    {
        "args": [
            [
                "flick",
                11037,
                3.14,
                53
            ]
        ],
        "return": [
            false,
            false,
            false,
            false
        ]
    },
    {
        "args": [
            [
                "flick",
                "flick",
                "flick",
                "flick",
                "flick"
            ]
        ],
        "return": [
            false,
            true,
            false,
            true,
            false
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
                [
                    "john",
                    "smith",
                    "susan"
                ],
                "flick"
            ]
        ],
        "return": [
            true,
            false
        ]
    },
    {
        "args": [
            [
                false,
                false,
                "flick",
                "sheep",
                "flick"
            ]
        ],
        "return": [
            true,
            true,
            false,
            false,
            true
        ]
    }
]
```
## Credits

Found on Edabit: [Flick Switch](https://edabit.com/challenge/YRwZvg5Pkgw4pEWC5)
