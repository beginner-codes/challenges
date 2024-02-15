# Challenge 823 - Tallest Skyscraper

A city skyline can be represented as a 2-D list with 1s representing buildings. In the example below, the height of the tallest building is 4 (second-most right column).
```python
[[0, 0, 0, 0, 0, 0],
[0, 0, 0, 0, 1, 0],
[0, 0, 1, 0, 1, 0],
[0, 1, 1, 1, 1, 0],
[1, 1, 1, 1, 1, 1]]
```
Create a function that takes a skyline (2-D list of 0's and 1's) and returns the height of the tallest skyscraper.

## Examples
```python
tallest_skyscraper([
  [0, 0, 0, 0],
  [0, 1, 0, 0],
  [0, 1, 1, 0],
  [1, 1, 1, 1]
]) ➞ 3

tallest_skyscraper([
  [0, 1, 0, 0],
  [0, 1, 0, 0],
  [0, 1, 1, 0],
  [1, 1, 1, 1]
]) ➞ 4

tallest_skyscraper([
  [0, 0, 0, 0],
  [0, 0, 0, 0],
  [1, 1, 1, 0],
  [1, 1, 1, 1]
]) ➞ 2
```
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


def tallest_skyscraper(skyline: list[list[int]]) -> int:
    return 0  # Put your code here!!!


test(823, tallest_skyscraper)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                [
                    0,
                    0,
                    0,
                    0,
                    0,
                    0
                ],
                [
                    0,
                    0,
                    0,
                    0,
                    0,
                    0
                ],
                [
                    1,
                    1,
                    1,
                    1,
                    0,
                    0
                ],
                [
                    1,
                    1,
                    1,
                    1,
                    1,
                    1
                ]
            ]
        ],
        "return": 2
    },
    {
        "args": [
            [
                [
                    0,
                    1,
                    0,
                    0
                ],
                [
                    0,
                    1,
                    0,
                    0
                ],
                [
                    0,
                    1,
                    1,
                    0
                ],
                [
                    1,
                    1,
                    1,
                    1
                ]
            ]
        ],
        "return": 4
    },
    {
        "args": [
            [
                [
                    0,
                    0,
                    0,
                    1
                ],
                [
                    0,
                    0,
                    0,
                    1
                ],
                [
                    1,
                    1,
                    1,
                    1
                ],
                [
                    1,
                    1,
                    1,
                    1
                ]
            ]
        ],
        "return": 4
    },
    {
        "args": [
            [
                [
                    0,
                    0,
                    0,
                    0
                ],
                [
                    0,
                    1,
                    0,
                    0
                ],
                [
                    0,
                    1,
                    1,
                    0
                ],
                [
                    1,
                    1,
                    1,
                    1
                ]
            ]
        ],
        "return": 3
    },
    {
        "args": [
            [
                [
                    0,
                    1,
                    0,
                    0,
                    0,
                    0
                ],
                [
                    0,
                    1,
                    0,
                    0,
                    0,
                    0
                ],
                [
                    0,
                    1,
                    0,
                    0,
                    0,
                    0
                ],
                [
                    1,
                    1,
                    1,
                    1,
                    0,
                    0
                ],
                [
                    1,
                    1,
                    1,
                    1,
                    1,
                    1
                ]
            ]
        ],
        "return": 5
    },
    {
        "args": [
            [
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
                ],
                [
                    1,
                    1,
                    1,
                    0
                ],
                [
                    1,
                    1,
                    1,
                    1
                ]
            ]
        ],
        "return": 2
    }
]
```

## Credits

Found on Edabit: [Tallest Skyscraper](https://edabit.com/challenge/76ibd8jZxvhAwDskb)
