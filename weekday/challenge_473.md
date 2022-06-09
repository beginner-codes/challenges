# Challenge 473 - Union and Intersection of Lists

Create a function that takes in two lists and returns an intersection list and a union list.

- Intersection List: Elements shared by both.
- Union List: Elements that exist in first or second list, or both (not exclusive OR).
- While the input lists may have duplicate numbers, the returned intersection and union lists should contain no duplicates. Returned lists should be sorted in ascending order.
```python
List 1: [5, 6, 6, 6, 8, 9]
List 2: [3, 3, 4, 4, 5, 5, 8]
```
- Intersection: `[5, 8]` - 5 and 8 are the only 2 numbers that exist in both lists.
- Union: `[3, 4, 5, 6, 8, 9]` -  Each number exists in at least one list.

## Examples
```python
intersection_union([1, 2, 3, 4, 4], [4, 5, 9]) ➞ [[4], [1, 2, 3, 4, 5, 9]]

intersection_union([1, 2, 3], [4, 5, 6]) ➞ [[], [1, 2, 3, 4, 5, 6]]

intersection_union([1, 1], [1, 1, 1, 1]) ➞ [[1], [1]]
```
## Notes

- Order of output should be:` [Intersection, Union]`.
- Remember both output lists should be in ascending order.
- If both lists are disjoint (share nothing in common), return an empty list for the intersection.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def intersection_union(list_a: list[int], list_b: list[int]) -> list[list[int]]:
    return []  # Put your code here!!!


test(473, intersection_union)  # Tell it which challenge to test against
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
                4,
                4
            ],
            [
                4,
                5,
                9
            ]
        ],
        "return": [
            [
                4
            ],
            [
                1,
                2,
                3,
                4,
                5,
                9
            ]
        ]
    },
    {
        "args": [
            [
                1,
                2,
                3
            ],
            [
                4,
                5,
                6
            ]
        ],
        "return": [
            [],
            [
                1,
                2,
                3,
                4,
                5,
                6
            ]
        ]
    },
    {
        "args": [
            [
                1,
                1
            ],
            [
                1,
                1,
                1,
                1
            ]
        ],
        "return": [
            [
                1
            ],
            [
                1
            ]
        ]
    },
    {
        "args": [
            [
                5,
                5
            ],
            [
                5,
                6
            ]
        ],
        "return": [
            [
                5
            ],
            [
                5,
                6
            ]
        ]
    },
    {
        "args": [
            [
                7,
                8,
                9,
                6
            ],
            [
                9,
                7,
                6,
                8
            ]
        ],
        "return": [
            [
                6,
                7,
                8,
                9
            ],
            [
                6,
                7,
                8,
                9
            ]
        ]
    }
]
```
## Credits

Found on Edabit: [Union and Intersection of Lists](https://edabit.com/challenge/Bb9PaM4B87L39SdAo)
