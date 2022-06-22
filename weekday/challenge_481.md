# Challenge 481 - Frequency Distribution

Create a function that returns the frequency distribution of a list. This function should return an object, where the keys are the unique elements and the values are the frequency in which those elements occur.

## Examples
```python
get_frequencies(["A", "B", "A", "A", "A"]) ➞ { "A" : 4, "B" : 1 }

get_frequencies([1, 2, 3, 3, 2]) ➞ { 1: 1, 2: 2, 3: 2 }

get_frequencies([True, False, True, False, False]) ➞ { True: 2, False: 3 }

get_frequencies([]) ➞ {}
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from typing import Hashable, TypeVar
from beginnercodes.challenges import test

T = TypeVar("T", bound=Hashable)

def get_frequencies(items: list[T]) -> dict[T, int]:
    return {}  # Put your code here!!!


test(481, get_frequencies)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "A",
                "A"
            ]
        ],
        "return": {
            "A": 2
        }
    },
    {
        "args": [
            [
                "A",
                "B",
                "A",
                "A",
                "A"
            ]
        ],
        "return": {
            "A": 4,
            "B": 1
        }
    },
    {
        "args": [
            [
                "A",
                "B",
                "C",
                "A",
                "A"
            ]
        ],
        "return": {
            "A": 3,
            "B": 1,
            "C": 1
        }
    },
    {
        "args": [
            [
                1,
                2,
                3,
                3,
                2
            ]
        ],
        "return": {
            "1": 1,
            "2": 2,
            "3": 2
        }
    },
    {
        "args": [
            [
                "true",
                "false",
                "true",
                "false",
                "false"
            ]
        ],
        "return": {
            "true": 2,
            "false": 3
        }
    },
    {
        "args": [
            []
        ],
        "return": {}
    }
]
```
## Credits

Found on Edabit: [Frequency Distribution](https://edabit.com/challenge/KKmM4ob5wwPwf8kgS)
