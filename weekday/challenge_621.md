# Challenge 621 - Movie Theater Seating

A group of friends is going to see a movie. They would like to find a spot where they can sit next to each other in the same row. A movie theater's seat layout can be represented as a 2-D matrix, where `0`s represent empty seats and `1`s represent taken seats.
```javascript
[[1, 0, 0, 0, 1, 1, 1],
[1, 1, 1, 0, 1, 1, 1],
[1, 0, 1, 0, 1, 0, 1],
[1, 1, 0, 1, 1, 0, 1],
[1, 0, 1, 1, 1, 1, 1],
[1, 0, 1, 1, 0, 0, 0]]
```
Create a function that, given a seat layout and the number of friends, returns the number of available spots where all of the friends can sit together. In the above example, if `n = 3`, there would be `2` spots (the first row and last row).

## Examples
```python
group_seats([
  [1, 0, 1, 0, 1, 0, 1],
  [0, 1, 0, 1, 0, 1, 0],
  [0, 0, 1, 1, 1, 1, 1],
  [1, 0, 1, 1, 0, 0, 1],
  [1, 1, 1, 0, 1, 0, 1],
  [0, 1, 1, 1, 1, 0, 0]
], 2) ➞ 3

group_seats([
  [1, 0, 1, 0, 1, 0, 1],
  [0, 1, 0, 0, 0, 0, 0],
], 4) ➞ 2
```
## Notes

- Multiple free arrangements that overlap still count as distinct arrangements

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def group_seats(seats: list[list[int]], num_friends: int) -> int:
    return 0  # Put your code here!!!


test(621, group_seats)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                [
                    1,
                    0,
                    0,
                    0,
                    1,
                    1,
                    1
                ],
                [
                    1,
                    1,
                    1,
                    0,
                    1,
                    1,
                    1
                ],
                [
                    1,
                    0,
                    1,
                    0,
                    1,
                    0,
                    1
                ],
                [
                    1,
                    1,
                    0,
                    1,
                    1,
                    0,
                    1
                ],
                [
                    1,
                    0,
                    1,
                    1,
                    1,
                    1,
                    1
                ],
                [
                    1,
                    0,
                    1,
                    1,
                    0,
                    0,
                    0
                ]
            ],
            3
        ],
        "return": 2
    },
    {
        "args": [
            [
                [
                    1,
                    0,
                    1,
                    0,
                    1,
                    0,
                    1
                ],
                [
                    0,
                    1,
                    0,
                    1,
                    0,
                    1,
                    0
                ],
                [
                    0,
                    0,
                    1,
                    1,
                    1,
                    1,
                    1
                ],
                [
                    1,
                    0,
                    1,
                    1,
                    0,
                    0,
                    1
                ],
                [
                    1,
                    1,
                    1,
                    0,
                    1,
                    0,
                    1
                ],
                [
                    0,
                    1,
                    1,
                    1,
                    1,
                    0,
                    0
                ]
            ],
            2
        ],
        "return": 3
    },
    {
        "args": [
            [
                [
                    1,
                    0,
                    1,
                    0,
                    0,
                    1,
                    1
                ],
                [
                    1,
                    1,
                    1,
                    0,
                    1,
                    1,
                    1
                ],
                [
                    1,
                    0,
                    1,
                    0,
                    1,
                    0,
                    1
                ],
                [
                    1,
                    1,
                    0,
                    1,
                    0,
                    0,
                    1
                ],
                [
                    1,
                    0,
                    1,
                    1,
                    1,
                    1,
                    1
                ],
                [
                    1,
                    0,
                    1,
                    1,
                    0,
                    0,
                    0
                ]
            ],
            2
        ],
        "return": 4
    },
    {
        "args": [
            [
                [
                    1,
                    0,
                    0,
                    0,
                    0,
                    1,
                    1
                ],
                [
                    1,
                    1,
                    1,
                    0,
                    1,
                    1,
                    1
                ],
                [
                    1,
                    0,
                    1,
                    0,
                    1,
                    0,
                    1
                ],
                [
                    1,
                    1,
                    0,
                    1,
                    1,
                    0,
                    1
                ],
                [
                    1,
                    0,
                    1,
                    1,
                    1,
                    1,
                    1
                ],
                [
                    1,
                    0,
                    1,
                    1,
                    0,
                    0,
                    0
                ]
            ],
            4
        ],
        "return": 1
    },
    {
        "args": [
            [
                [
                    1,
                    0,
                    1,
                    0,
                    1,
                    0,
                    1
                ],
                [
                    0,
                    1,
                    0,
                    0,
                    0,
                    0,
                    0
                ]
            ],
            4
        ],
        "return": 2
    }
]
```
## Credits

Found on Edabit: [Movie Theater Seating](https://edabit.com/challenge/dKeLAqAxpddbkvNhh)
