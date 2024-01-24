# Challenge 810 - Generating and Swapping Key-Value-Pairs in Dictionary

Create a function that takes:

- A list of string keys
- A list of string values
- True, if key and value should be swapped, else False

The function returns the constructed dict. Empty lists return an empty dict.

## Examples
```python
swap_d(["1", "2", "3"], ["one", "two", "three"], False)
➞ {"1": "one", "2": "two", "3": "three"}

swap_d(["1", "2", "3"], ["one", "two", "three"], True)
➞ {"one": "1", "two": "2", "three": "3"}

swap_d(["Paris", "3", "4.5"], ["France", "is odd", "is half of 9"], True)
➞ {"France": "Paris", "is odd": "3", "is half of 9": "4.5"}
```
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


def swap_d(keys: list[str], values: list[str], swap: bool) -> dict[str, str]:
    return {}  # Put your code here!!!


test(810, swap_d)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                "(1, 2)",
                "(3, 4)",
                "(5, 6)"
            ],
            [
                "one_two",
                "three_four",
                "five_six"
            ],
            false
        ],
        "return": {
            "(1, 2)": "one_two",
            "(3, 4)": "three_four",
            "(5, 6)": "five_six"
        }
    },
    {
        "args": [
            [
                "1",
                "2",
                "3"
            ],
            [
                "one",
                "two",
                "three"
            ],
            false
        ],
        "return": {
            "1": "one",
            "2": "two",
            "3": "three"
        }
    },
    {
        "args": [
            [
                "(1, 2)",
                "(3, 4)",
                "(5, 6)"
            ],
            [
                "one_two",
                "three_four",
                "five_six"
            ],
            true
        ],
        "return": {
            "one_two": "(1, 2)",
            "three_four": "(3, 4)",
            "five_six": "(5, 6)"
        }
    },
    {
        "args": [
            [
                "Paris",
                "Berlin",
                "Washington"
            ],
            [
                "France",
                "Germany",
                "USA"
            ],
            true
        ],
        "return": {
            "France": "Paris",
            "Germany": "Berlin",
            "USA": "Washington"
        }
    },
    {
        "args": [
            [],
            [],
            false
        ],
        "return": {}
    }
]
```

## Credits

Found on Edabit: [Generating and Swapping Key-Value-Pairs in Dictionary](https://edabit.com/challenge/cEzT2e8tLpwYnrstP)
