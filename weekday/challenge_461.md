# Challenge 461 - Negative Image

Suppose an image can be represented as a 2D list of `0`s and `1`s. Create a function to reverse an image. Replace the `0`s with `1`s and vice versa.

## Examples
```python
reverse_image([
  [1, 0, 0],
  [0, 1, 0],
  [0, 0, 1]
]) ➞ [
  [0, 1, 1],
  [1, 0, 1],
  [1, 1, 0]
]

reverse_image([
  [1, 1, 1],
  [0, 0, 0]
]) ➞ [
  [0, 0, 0],
  [1, 1, 1]
]

reverse_image([
  [1, 0, 0],
  [1, 0, 0]
]) ➞ [
  [0, 1, 1],
  [0, 1, 1]
]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from beginnercodes.challenges import test


def reverse_image(image: list[list[int]]) -> list[list[int]]:
    return []  # Put your code here!!!


test(461, reverse_image)  # Tell it which challenge to test against
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
                    0
                ],
                [
                    0,
                    1,
                    0
                ],
                [
                    0,
                    0,
                    1
                ]
            ]
        ],
        "return": [
            [
                0,
                1,
                1
            ],
            [
                1,
                0,
                1
            ],
            [
                1,
                1,
                0
            ]
        ]
    },
    {
        "args": [
            [
                [
                    1,
                    1,
                    1
                ],
                [
                    0,
                    0,
                    0
                ]
            ]
        ],
        "return": [
            [
                0,
                0,
                0
            ],
            [
                1,
                1,
                1
            ]
        ]
    },
    {
        "args": [
            [
                [
                    1,
                    0,
                    0
                ],
                [
                    1,
                    0,
                    0
                ]
            ]
        ],
        "return": [
            [
                0,
                1,
                1
            ],
            [
                0,
                1,
                1
            ]
        ]
    },
    {
        "args": [
            [
                [
                    1,
                    0,
                    0,
                    0,
                    0
                ],
                [
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
                    1,
                    1
                ],
                [
                    1,
                    1,
                    1,
                    1,
                    0
                ],
                [
                    1,
                    1,
                    1,
                    0,
                    0
                ]
            ]
        ],
        "return": [
            [
                0,
                1,
                1,
                1,
                1
            ],
            [
                0,
                1,
                1,
                0,
                0
            ],
            [
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
                1
            ],
            [
                0,
                0,
                0,
                1,
                1
            ]
        ]
    },
    {
        "args": [
            [
                [
                    1,
                    1
                ],
                [
                    1,
                    0
                ],
                [
                    1,
                    1
                ],
                [
                    1,
                    1
                ],
                [
                    1,
                    1
                ]
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
                0
            ],
            [
                0,
                0
            ],
            [
                0,
                0
            ]
        ]
    }
]
```
## Credits

Found on Edabit: [Negative Image](https://edabit.com/challenge/cAYMDMFgTHuZJw2o4)
