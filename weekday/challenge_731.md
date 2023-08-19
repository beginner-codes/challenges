# Challenge 731 - Are Pairs Sufficient for a Clear Ordering?

Create a function that returns True if an array of pairs is sufficient for a clear ordering of all items. In each pair the first item evaluates to less than the second item.

To illustrate:
```python
clear_ordering([["D", "A"], ["C", "B"], ["A", "C"]]) ➞ True
# Since unequivocally: "D" < "A" < "C" < "B"
```
On the other hand:
```python
clear_ordering([["D", "A"], ["B", "A"], ["C", "D"]]) ➞ False
# Since we know that "C" < "D" < "A", and we know "B" < "A"
# but we don't know anything about "B"s relationship with "C" or "D".
```
## Examples
```.python
clear_ordering([["S", "T"], ["T", "U"], ["U", "V"]]) ➞ True

clear_ordering([["T", "S"], ["T", "U"], ["U", "V"], ["V", "W"]]) ➞ False
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def clear_ordering(orderings: list[str]) -> bool:
    return False  # Put your code here!!!


test(731, clear_ordering)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                [
                    "A",
                    "D"
                ],
                [
                    "C",
                    "D"
                ]
            ]
        ],
        "return": false
    },
    {
        "args": [
            [
                [
                    "b",
                    "a"
                ],
                [
                    "b",
                    "c"
                ],
                [
                    "c",
                    "d"
                ],
                [
                    "e",
                    "f"
                ],
                [
                    "d",
                    "e"
                ]
            ]
        ],
        "return": false
    },
    {
        "args": [
            [
                [
                    "A",
                    "D"
                ],
                [
                    "D",
                    "C"
                ]
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                [
                    "D",
                    "A"
                ],
                [
                    "C",
                    "B"
                ],
                [
                    "A",
                    "C"
                ]
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                [
                    "d",
                    "c"
                ],
                [
                    "a",
                    "b"
                ],
                [
                    "b",
                    "c"
                ]
            ]
        ],
        "return": false
    }
]
```
## Credits

Found on Edabit: [Are Pairs Sufficient for a Clear Ordering?](https://edabit.com/challenge/CdcS3feCCEHxtDr2a)
