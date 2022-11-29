# Challenge 579 - Intersection of Two Dictionaries

Write a function that takes as input two different dictionaries and filters the keys in each dictionary to only keep keys that exist in both dictionaries. Store your result as a list with two dictionaries.

## Examples
```python
dict1 = {"a": 5, "b": 13, "c": 7}
dict2 = {"b": 5, "c": 8, "d": 91, "e": 99}
dict3 = {"a": 1, "b": 34}
dict4 = {"c": 9, "d": 8}

intersection(dict1, dict2) ➞ [{"b": 13, "c": 7}, {"b": 5, "c": 8}]

intersection(dict1, dict4) ➞ [{"c": 7}, {"c": 9}]

intersection(dict3, dict4) ➞ [{}, {}]
```
## Notes

- If no keys are shared between both dictionaries, return a list of empty dictionaries.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def intersection(d1: dict[str, int], d2: dict[str, int]) -> list[dict[str, int]]:
    return []  # Put your code here!!!


test(579, intersection)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            {
                "a": 5,
                "b": 13,
                "c": 7
            },
            {
                "b": 5,
                "c": 8,
                "d": 91,
                "e": 99
            }
        ],
        "return": [
            {
                "b": 13,
                "c": 7
            },
            {
                "b": 5,
                "c": 8
            }
        ]
    },
    {
        "args": [
            {
                "a": 1,
                "b": 34
            },
            {
                "c": 9,
                "d": 8
            }
        ],
        "return": [
            {},
            {}
        ]
    },
    {
        "args": [
            {
                "a": 5,
                "b": 13,
                "c": 7
            },
            {
                "c": 9,
                "d": 8
            }
        ],
        "return": [
            {
                "c": 7
            },
            {
                "c": 9
            }
        ]
    },
    {
        "args": [
            {
                "a": 5,
                "b": 13,
                "c": 7
            },
            {
                "a": 1,
                "b": 34
            }
        ],
        "return": [
            {
                "a": 5,
                "b": 13
            },
            {
                "a": 1,
                "b": 34
            }
        ]
    }
]
```
## Credits

Found on Edabit: [Intersection of Two Dictionaries](https://edabit.com/challenge/Hg2gFcJDg7Rz5bd5m)
