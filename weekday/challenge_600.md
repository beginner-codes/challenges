# Challenge 600 - Postman Harry

Harry is a postman. He's got a post office with a size of `n*m` (a matrix/2D list). Each slot at the 2D list represents the number of letters in that spot. Harry can only go right and down. He starts at `(0, 0)`, and ends at `(n-1, m-1)`. `n` represents the height, and `m` the length. Return the maximum amount of letters he can pick up. He can only pick up letters if he is on that spot.

## Examples
```python
harry([[5, 2], [5, 2]]) ➞ 12
# (5+5+2)


harry([
  [1, 2, 3, 4, 5],
  [6, 7, 8, 9, 10],
  [11, 12, 13, 14, 15]
]) ➞ 72
# (1+6+11+12+13+14+15)


harry([[]]) ➞ -1
```
## Notes

- If the matrix is empty, return `-1`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def harry(post_office: list[list[int]]) -> int:
    return 0  # Put your code here!!!


test(600, harry)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                [
                    5,
                    2
                ],
                [
                    5,
                    2
                ],
                [
                    5,
                    2
                ],
                [
                    5,
                    2
                ]
            ]
        ],
        "return": 22
    },
    {
        "args": [
            [
                []
            ]
        ],
        "return": -1
    },
    {
        "args": [
            [
                [
                    5,
                    6,
                    2,
                    5,
                    1
                ],
                [
                    7,
                    2,
                    4,
                    1,
                    2
                ],
                [
                    0,
                    7,
                    5,
                    2,
                    14
                ],
                [
                    9,
                    5,
                    12,
                    5,
                    9
                ],
                [
                    19,
                    5,
                    2,
                    6,
                    2
                ]
            ]
        ],
        "return": 55
    },
    {
        "args": [
            [
                [
                    9,
                    9,
                    9
                ],
                [
                    0,
                    0,
                    9
                ],
                [
                    0,
                    0,
                    9
                ]
            ]
        ],
        "return": 45
    },
    {
        "args": [
            [
                [
                    5
                ]
            ]
        ],
        "return": 5
    }
]
```
## Credits

Found on Edabit: [Postman Harry](https://edabit.com/challenge/7yo5FJX4xFbNxim5q)
