# Challenge 794 - Generate N-Size Combinations from a List

Create a function that returns all combinations of size `n` from a list. Sort the list in ascending lexicographical order.

## Examples
```python
combo([1, 2, 3, 4], 1) ➞ [[1], [2], [3], [4]]

combo([1, 2, 3, 4], 2) ➞ [[1, 2], [1, 3], [1, 4], [2, 3], [2, 4], [3, 4]]

combo([1, 2, 3, 4], 5) ➞ []

combo([1, 2, 3, 4], 0) ➞ [[]]
```
## Notes

- Lexicographical order: Compare the first element: `[1, 2]` will be before `[2, 4]`. If both share the same first element, compare the second element: `[1, 2]` is before `[1, 3]`, etc.
- Return an empty list if `n` exceeds the length of the list.
- Return `[[]]` if `n` is 0.

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


def combo(items: list[int], n: int) -> list[list[int]]:
    return []  # Put your code here!!!


test(794, combo)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                1,
                2,
                3,
                4
            ],
            3
        ],
        "return": [
            [
                1,
                2,
                3
            ],
            [
                1,
                2,
                4
            ],
            [
                1,
                3,
                4
            ],
            [
                2,
                3,
                4
            ]
        ]
    },
    {
        "args": [
            [
                1,
                2,
                3,
                4
            ],
            0
        ],
        "return": [
            []
        ]
    },
    {
        "args": [
            [
                1,
                2,
                3,
                4
            ],
            5
        ],
        "return": []
    },
    {
        "args": [
            [
                1,
                2,
                3,
                4
            ],
            1
        ],
        "return": [
            [
                1
            ],
            [
                2
            ],
            [
                3
            ],
            [
                4
            ]
        ]
    }
]
```

## Credits

Found on Edabit: [Generate N-Size Combinations from a List](https://edabit.com/challenge/hD8vgeNkjXy5trX6h)
