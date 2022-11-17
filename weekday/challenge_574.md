# Challenge 574 - Merge Two Lists

Create a function that takes two lists and combines them by alternating elements from each list.

- The lists may be of different lengths.
- The first list will contain string characters (lowercase, `a-z`).
- The second list will contain integers (all positive).

## Examples
```python
merge_arrays(["a", "b", "c", "d", "e"], [1, 2, 3, 4, 5])
➞ ["a", 1, "b", 2, "c", 3, "d", 4, "e", 5]

merge_arrays([1, 2, 3], ["a", "b", "c", "d", "e", "f"])
➞ [1, "a", 2, "b", 3, "c", "d", "e", "f"]

merge_arrays(["f", "d", "w", "t"], [5, 3, 7, 8])
➞ ["f", 5, "d", 3, "w", 7, "t", 8]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def merge_arrays(strings: list[str], numbers: list[int]) -> list[str | int]:
    return []  # Put your code here!!!


test(574, merge_arrays)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "a",
                "b",
                "c",
                "d",
                "e"
            ],
            [
                1,
                2,
                3,
                4,
                5
            ]
        ],
        "return": [
            "a",
            1,
            "b",
            2,
            "c",
            3,
            "d",
            4,
            "e",
            5
        ]
    },
    {
        "args": [
            [
                123,
                456
            ],
            [
                "c",
                "b",
                "a"
            ]
        ],
        "return": [
            123,
            "c",
            456,
            "b",
            "a"
        ]
    },
    {
        "args": [
            [
                "c"
            ],
            [
                3
            ]
        ],
        "return": [
            "c",
            3
        ]
    },
    {
        "args": [
            [
                "f",
                "d",
                "w",
                "t"
            ],
            [
                5,
                3,
                7,
                8
            ]
        ],
        "return": [
            "f",
            5,
            "d",
            3,
            "w",
            7,
            "t",
            8
        ]
    },
    {
        "args": [
            [
                4,
                3,
                2,
                1
            ],
            [
                "r",
                "d"
            ]
        ],
        "return": [
            4,
            "r",
            3,
            "d",
            2,
            1
        ]
    }
]
```
## Credits

Found on Edabit: [Directionally ChallengedMerge Two Lists](https://edabit.com/challenge/q7BdzRw4j7zFfFb4R)
