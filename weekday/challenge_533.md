# Challenge 533 - All Subsets that Add to a Value 

Create a function that returns all sublists in a list that sum to a particular value. Return the sublists in the following order:

- First by ascending length.
- Second by comparing element-by-element, starting from the leftmost one. Put the list with the smaller element first in the pairwise comparison.

The following example will illustrate:
```python
get_subsets([-3, -2, -1, 0, 1, 2, 3], 2)
[ # All the subsets below sum to 2.
  [2],
  [-1, 3],
  [0, 2], # Same length: -1 < 0, so [-1, 3] goes before [0, 2]
  [-3, 2, 3],
  [-2, 1, 3],
  [-1, 0, 3],
  [-1, 1, 2],
  [-3, 0, 2, 3],
  [-2, -1, 2, 3],
  [-2, 0, 1, 3], # Same length + same first element: -1 < 0, so [-2, -1, 2, 3] goes before [-2, 0, 1, 3]
  [-1, 0, 1, 2],
  [-3, -1, 1, 2, 3],
  [-2, -1, 0, 2, 3],
  [-3, -1, 0, 1, 2, 3]
]
```
## Examples
```python
get_subsets([-1, 0, 1, 2], 2) ➞ [[2], [0, 2], [-1, 1, 2], [-1, 0, 1, 2]]

get_subsets([-1, 0, 1, 2], 3) ➞ [[1, 2], [0, 1, 2]]

get_subsets([1, 2, 3, 4], 5) ➞ [[1, 4], [2, 3]]

get_subsets([-1, 0, 1, 2], 4) ➞ []
```
## Notes

- Lists will have unique numbers.
- Return an empty list if there does not exist a subset that sums to the given value.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def get_subsets(numbers: list[int], value: int) -> list[list[int]]:
    return [] # Put your code here!!!


test(533, get_subsets)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                -1,
                0,
                1,
                2
            ],
            4
        ],
        "return": []
    },
    {
        "args": [
            [
                -1,
                0,
                1,
                2
            ],
            2
        ],
        "return": [
            [
                2
            ],
            [
                0,
                2
            ],
            [
                -1,
                1,
                2
            ],
            [
                -1,
                0,
                1,
                2
            ]
        ]
    },
    {
        "args": [
            [
                1,
                2,
                3,
                4,
                5,
                6
            ],
            6
        ],
        "return": [
            [
                6
            ],
            [
                1,
                5
            ],
            [
                2,
                4
            ],
            [
                1,
                2,
                3
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
            ]
        ]
    },
    {
        "args": [
            [
                -1,
                0,
                1,
                2
            ],
            3
        ],
        "return": [
            [
                1,
                2
            ],
            [
                0,
                1,
                2
            ]
        ]
    }
]
```
## Credits

Found on Edabit: [All Subsets that Add to a Value](https://edabit.com/challenge/FnyAGdwgcH4whynjR)
