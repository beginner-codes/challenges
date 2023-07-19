# Challenge 708 - Get Students with Names and Notes Average

Create a function that takes a list of user mappings that contain their name and a list of note values and that returns a list of mappings that contain the users' names and the average note value. If a student has no notes then the average should be 0.

## Examples
```python
average_note([
  { "name": "John", "notes": [3, 5, 4]}
]) ➞ [
  { "name": "John", "avgNote": 4 }
]

average_note([
  { "name": "John", "notes": [7, 8, 6]},
  { "name": "Jane", "notes": [1, 2, 3]},
]) ➞ [
  { "name": "John", "avgNote": 7 },
  { "name": "Jane", "avgNote": 2 },
]
```
## Notes

- Round the average to a whole number.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def average_notes(students: list[dict[str, str | list[int]]]) -> list[dict[str, str | int]]:
    return []  # Put your code here!!!


test(708, average_notes)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                {
                    "name": "Solo",
                    "notes": []
                }
            ]
        ],
        "return": [
            {
                "name": "Solo",
                "avgNote": 0
            }
        ]
    },
    {
        "args": [
            [
                {
                    "name": "Victor",
                    "notes": [
                        1,
                        3,
                        5
                    ]
                }
            ]
        ],
        "return": [
            {
                "name": "Victor",
                "avgNote": 3
            }
        ]
    },
    {
        "args": [
            [
                {
                    "name": "Paul",
                    "notes": []
                },
                {
                    "name": "Victoria",
                    "notes": [
                        3,
                        5,
                        2,
                        1
                    ]
                }
            ]
        ],
        "return": [
            {
                "name": "Paul",
                "avgNote": 0
            },
            {
                "name": "Victoria",
                "avgNote": 3
            }
        ]
    },
    {
        "args": [
            [
                {
                    "name": "John",
                    "notes": [
                        2,
                        4,
                        5
                    ]
                },
                {
                    "name": "Mich",
                    "notes": [
                        1,
                        3,
                        5
                    ]
                }
            ]
        ],
        "return": [
            {
                "name": "John",
                "avgNote": 4
            },
            {
                "name": "Mich",
                "avgNote": 3
            }
        ]
    },
    {
        "args": [
            [
                {
                    "name": "Vicky",
                    "notes": [
                        5,
                        4
                    ]
                },
                {
                    "name": "Sanders",
                    "notes": [
                        4,
                        3,
                        4
                    ]
                }
            ]
        ],
        "return": [
            {
                "name": "Vicky",
                "avgNote": 4
            },
            {
                "name": "Sanders",
                "avgNote": 4
            }
        ]
    }
]
```
## Credits

Found on Edabit: [Get Students with Names and Notes Average](https://edabit.com/challenge/nqNWZ7ayzZoRMZu8Z)
