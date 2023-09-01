# Challenge 741 - Bridge Shuffle

Create a function to bridge shuffle two lists. To bridge shuffle, you interleave the elements from both lists in an alternating fashion, like so:
```python
List 1 = ["A", "A", "A"]
List 2 = ["B", "B", "B"]

Shuffled List = ["A", "B", "A", "B", "A", "B"]
```
This can still work with two lists of uneven length. We simply tack on the extra elements from the longer list, like so:
```python
List 1 = ["C", "C", "C", "C"]
List 2 = ["D"]

Shuffled List = ["C", "D", "C", "C", "C"]
```
Create a function that takes in two lists and returns the bridge-shuffled list.

## Examples
```python
bridge_shuffle(["A", "A", "A"], ["B", "B", "B"]) ➞ ["A", "B", "A", "B", "A", "B"]

bridge_shuffle(["C", "C", "C", "C"], ["D"]) ➞ ["C", "D", "C", "C", "C"]

bridge_shuffle([1, 3, 5, 7], [2, 4, 6]) ➞ [1, 2, 3, 4, 5, 6, 7]
```
## Notes

- Elements in both lists can be strings or integers.
- If two lists are of unequal length, add the additional elements of the longer list to the end of the shuffled list.
- Always start your shuffle with the first element of List 1.

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
from typing import TypeVar


T = TypeVar("T")


def bridge_shuffle(list_1: list[T], list_2: list[T]) -> list[T]:
    return []  # Put your code here!!!


test(741, bridge_shuffle)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                "A",
                "A",
                "A"
            ],
            [
                "B",
                "B",
                "B"
            ]
        ],
        "return": [
            "A",
            "B",
            "A",
            "B",
            "A",
            "B"
        ]
    },
    {
        "args": [
            [
                "C",
                "C",
                "C",
                "C"
            ],
            [
                "D"
            ]
        ],
        "return": [
            "C",
            "D",
            "C",
            "C",
            "C"
        ]
    },
    {
        "args": [
            [
                1,
                3,
                5,
                7
            ],
            [
                2,
                4,
                6
            ]
        ],
        "return": [
            1,
            2,
            3,
            4,
            5,
            6,
            7
        ]
    },
    {
        "args": [
            [
                "h",
                "h",
                "h"
            ],
            [
                "a",
                "a",
                "a"
            ]
        ],
        "return": [
            "h",
            "a",
            "h",
            "a",
            "h",
            "a"
        ]
    },
    {
        "args": [
            [
                10,
                9,
                8
            ],
            [
                1,
                2,
                3,
                4
            ]
        ],
        "return": [
            10,
            1,
            9,
            2,
            8,
            3,
            4
        ]
    }
]
```

## Credits

Found on Edabit: [Simple Row Sum](https://edabit.com/challenge/ysgbRFTPujx8v37yF)
