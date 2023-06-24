# Challenge 692 - Ordering People in a Line

Create a function that takes in the size of the line and the number of people waiting and places people in an S-shape ordering. The demonstration below will make it clear:
```python
# Ordering numbers 1-15 in a [5,3] space.

order_people([5, 3], 15) ➞ [
  [1, 2, 3],
  [6, 5, 4],
  [7, 8, 9],
  [12, 11, 10],
  [13, 14, 15]
]
```
If there is extra room, leave those spots blank with a 0 filler.
```python
# Ordering numbers 1-5 in a [4, 3] space.

order_people([4, 3], 5) ➞ [
  [1, 2, 3],
  [0, 5, 4],
  [0, 0, 0],
  [0, 0, 0]
]
```
If there are too many people for the given dimensions, return `"overcrowded"`.
```python
order_people([4, 3], 20) ➞ "overcrowded"
```
## Examples
```python
order_people([3, 3], 8) ➞ [
  [1, 2, 3],
  [6, 5, 4],
  [7, 8, 0]
]

order_people([2, 4], 5) ➞ [
  [1, 2, 3, 4],
  [0, 0, 0, 5]
]

order_people([2, 4], 10) ➞ "overcrowded"
```
## Notes

- Always start the ordering in the upper-left corner.
- If the S-shape concept doesn't make sense, try writing down some of these examples on a piece of paper and tracing a pencil through the numbers in order.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def order_people(line: list[int], number_people: int) -> list[list[int]]:
    return []  # Put your code here!!!


test(692, order_people)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                2,
                2
            ],
            4
        ],
        "return": [
            [
                1,
                2
            ],
            [
                4,
                3
            ]
        ]
    },
    {
        "args": [
            [
                3,
                4
            ],
            1
        ],
        "return": [
            [
                1,
                0,
                0,
                0
            ],
            [
                0,
                0,
                0,
                0
            ],
            [
                0,
                0,
                0,
                0
            ]
        ]
    },
    {
        "args": [
            [
                2,
                2
            ],
            5
        ],
        "return": "overcrowded"
    },
    {
        "args": [
            [
                5,
                3
            ],
            15
        ],
        "return": [
            [
                1,
                2,
                3
            ],
            [
                6,
                5,
                4
            ],
            [
                7,
                8,
                9
            ],
            [
                12,
                11,
                10
            ],
            [
                13,
                14,
                15
            ]
        ]
    },
    {
        "args": [
            [
                4,
                3
            ],
            5
        ],
        "return": [
            [
                1,
                2,
                3
            ],
            [
                0,
                5,
                4
            ],
            [
                0,
                0,
                0
            ],
            [
                0,
                0,
                0
            ]
        ]
    }
]
```
## Credits

Found on Edabit: [Ordering People in a Line](https://edabit.com/challenge/Pf2kDoCRvEL8qzKTs)
