# Challenge 563 - Sliding Sum

Create a function that returns the subarrays of `n` consecutive elements that sum up to `k`. The function will have the following form: `sliding_sum(lst, n, k)`

To illustrate:
```python
sliding_sum([3, 4, 1, 9, 9, 0, 3, 5, 4], 3, 8) ➞ [[3, 4, 1], [0, 3, 5]]
# Where [3, 4, 1] and [0, 3, 5] are the only subarrays that sum to 8 with length 3.
```
## Examples
```python
sliding_sum([1, 4, 2, 3, 5, 0], 2, 5) ➞ [[1, 4], [2, 3], [5, 0]]

sliding_sum([5, 5, 5, 5, 5], 1, 5) ➞ [[5], [5], [5], [5], [5]]

sliding_sum([5, 5, 5, 5, 5], 5, 24) ➞ []
```
## Notes

- Return an empty array if no subarrays satisfy the `(n,k)` condition.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def sliding_sum(lst: list[int], n: int, k: int) -> list[list[int]]:
    return [] # Put your code here!!!


test(563, sliding_sum)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                1,
                4,
                2,
                3,
                5,
                0
            ],
            2,
            5
        ],
        "return": [
            [
                1,
                4
            ],
            [
                2,
                3
            ],
            [
                5,
                0
            ]
        ]
    },
    {
        "args": [
            [
                3,
                2,
                1,
                1,
                3,
                2
            ],
            4,
            7
        ],
        "return": [
            [
                3,
                2,
                1,
                1
            ],
            [
                2,
                1,
                1,
                3
            ],
            [
                1,
                1,
                3,
                2
            ]
        ]
    },
    {
        "args": [
            [
                3,
                4,
                1,
                9,
                9,
                0,
                3,
                5,
                4
            ],
            3,
            8
        ],
        "return": [
            [
                3,
                4,
                1
            ],
            [
                0,
                3,
                5
            ]
        ]
    },
    {
        "args": [
            [
                5,
                5,
                5,
                5,
                5
            ],
            5,
            24
        ],
        "return": []
    },
    {
        "args": [
            [
                5,
                5,
                5,
                5,
                5
            ],
            1,
            5
        ],
        "return": [
            [
                5
            ],
            [
                5
            ],
            [
                5
            ],
            [
                5
            ],
            [
                5
            ]
        ]
    }
]
```
## Credits

Found on Edabit: [Sliding Sum](https://edabit.com/challenge/PbucHZpWm6ZGEtqki)
