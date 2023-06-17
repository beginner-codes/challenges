# Challenge 687 - Fit the Pattern 

Create a function that checks if the sub-lists in a list adhere to a given pattern.

## Examples
```python
check_pattern([[1, 1], [2, 2], [1, 1], [2, 2]], "ABAB") ➞ True

check_pattern([[1, 2], [1, 3], [1, 4], [1, 2]], "ABCA") ➞ True

check_pattern([[1, 2, 3], [1, 2, 3], [3, 2, 1], [3, 2, 1]], "AABB") ➞ True

check_pattern([[8, 8, 8, 8], [7, 7, 7, 7], [6, 6, 6, 6], [5, 5, 5, 5]], "ABCD") ➞ True

check_pattern([[8, 8, 8, 8], [7, 7, 7, 7], [6, 6, 6, 6], [5, 5, 5, 5]], "DCBA") ➞ True
```
## Notes

- The length of the pattern will always be the same as the length of the (main) list.
- The pattern does not necessarily have to be alphabetically ordered.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def check_pattern(lists: list[list[int]], pattern: str) -> bool:
    return False  # Put your code here!!!


test(687, check_pattern)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                [
                    1,
                    2
                ],
                [
                    1,
                    2
                ],
                [
                    2,
                    2
                ],
                [
                    3,
                    2
                ]
            ],
            "AAAA"
        ],
        "return": false
    },
    {
        "args": [
            [
                [
                    8,
                    8,
                    8,
                    8
                ],
                [
                    7,
                    7,
                    7,
                    7
                ],
                [
                    6,
                    6,
                    6,
                    6
                ],
                [
                    5,
                    5,
                    5,
                    5
                ]
            ],
            "ABCD"
        ],
        "return": true
    },
    {
        "args": [
            [
                [
                    8
                ],
                [
                    9
                ],
                [
                    9
                ],
                [
                    9
                ]
            ],
            "ABBB"
        ],
        "return": true
    },
    {
        "args": [
            [
                [
                    8,
                    8,
                    8,
                    8
                ],
                [
                    7,
                    7,
                    7,
                    7
                ],
                [
                    6,
                    6,
                    6,
                    6
                ],
                [
                    5,
                    5,
                    5,
                    5
                ]
            ],
            "DDBA"
        ],
        "return": false
    },
    {
        "args": [
            [
                [
                    8,
                    8,
                    8,
                    8
                ],
                [
                    7,
                    7,
                    7,
                    7
                ],
                [
                    6,
                    6,
                    6,
                    6
                ],
                [
                    5,
                    5,
                    5,
                    5
                ]
            ],
            "DCBA"
        ],
        "return": true
    }
]
```
## Credits

Found on Edabit: [Fit the Pattern](https://edabit.com/challenge/z9tnydD5Fix3g3mas)
