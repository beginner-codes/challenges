# Challenge 613 - Subset of a Cartesian Product


Write a function which takes a list of numbers and returns a list of tuples that is a subset of product of the list with itself and first member of each tuple is less than or equal to the second one.

In mathematical terms:
```
A x A = {(x,y)| x∈A and y∈A}

{(x,y)| x>=y, (x,y) ∈ A x A }
```
## Examples
```python
relation_list([0, 1, 2, 3]) ➞ [[0, 0], [0, 1], [0, 2], [0, 3], [1, 1], [1, 2], [1, 3], [2, 2], [2, 3]]

relation_lst([858, 544, 164]) ➞ [[164, 164], [164, 544], [164, 858], [544, 544], [544, 858], [858, 858]]

relation_lst([-1]) ➞ [[-1, -1]]

relation_lst([0]) ➞ [[0, 0]]

relation_lst([]), []
```
## Notes

- The result should be in ascending order.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def relation_lst(numbers: list[int]) -> list[list[int]]:
    return []  # Put your code here!!!


test(613, relation_lst)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                -1
            ]
        ],
        "return": [
            [
                -1,
                -1
            ]
        ]
    },
    {
        "args": [
            []
        ],
        "return": []
    },
    {
        "args": [
            [
                806,
                586,
                788,
                440
            ]
        ],
        "return": [
            [
                440,
                440
            ],
            [
                440,
                586
            ],
            [
                440,
                788
            ],
            [
                440,
                806
            ],
            [
                586,
                586
            ],
            [
                586,
                788
            ],
            [
                586,
                806
            ],
            [
                788,
                788
            ],
            [
                788,
                806
            ],
            [
                806,
                806
            ]
        ]
    },
    {
        "args": [
            [
                0,
                1,
                2,
                3
            ]
        ],
        "return": [
            [
                0,
                0
            ],
            [
                0,
                1
            ],
            [
                0,
                2
            ],
            [
                0,
                3
            ],
            [
                1,
                1
            ],
            [
                1,
                2
            ],
            [
                1,
                3
            ],
            [
                2,
                2
            ],
            [
                2,
                3
            ],
            [
                3,
                3
            ]
        ]
    }
]
```
## Credits

Found on Edabit: [Subset of a Cartasian Product](https://edabit.com/challenge/H6J4o4jqGbffYXe3Y)
