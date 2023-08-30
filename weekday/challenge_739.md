# Challenge 739 - Get the Diagonals

Given a square matrix implement a function that returns a containing two lists equal to the two diagonals, in the
following order:

- diagonal 1 = from upper-left to lower-right corner
- diagonal 2 = from upper-right to lower-left corner

## Examples

```python
get_diagonals([[1, 2], [3, 4]]) ➞ [[1, 4], [2, 3]]

get_diagonals([["a", "b", "c"], ["d", "e", "f"], ["g", "h", "i"]]) ➞ [["a", "e", "i"], ["c", "e", "g"]]

get_diagonals([[True]]) ➞ [[True], [True]]
```

## Notes

- Your function must also work with single elements or empty lists.
- Try to build both diagonals with a single loop.

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
from typing import TypeVar


T = TypeVar("T")


def get_diagonals(matrix: list[list[T]]) -> list[list[T]]:
    return []  # Put your code here!!!


test(739, get_diagonals)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
  {
    "args": [
      []
    ],
    "return": [
      [],
      []
    ]
  },
  {
    "args": [
      [
        [
          1,
          2,
          3
        ],
        [
          4,
          5,
          6
        ],
        [
          7,
          8,
          9
        ]
      ]
    ],
    "return": [
      [
        1,
        5,
        9
      ],
      [
        3,
        5,
        7
      ]
    ]
  },
  {
    "args": [
      [
        [
          "e",
          "z",
          "y",
          "o",
          "p",
          "t"
        ],
        [
          "b",
          "d",
          "a",
          "t",
          "i",
          "w"
        ],
        [
          "u",
          "l",
          "a",
          "n",
          "s",
          "k"
        ],
        [
          "s",
          "v",
          "k",
          "b",
          "r",
          "z"
        ],
        [
          "h",
          "e",
          "w",
          "c",
          "i",
          "j"
        ],
        [
          "r",
          "p",
          "y",
          "d",
          "x",
          "t"
        ]
      ]
    ],
    "return": [
      [
        "e",
        "d",
        "a",
        "b",
        "i",
        "t"
      ],
      [
        "t",
        "i",
        "n",
        "k",
        "e",
        "r"
      ]
    ]
  },
  {
    "args": [
      [
        [
          "Trivial"
        ]
      ]
    ],
    "return": [
      [
        "Trivial"
      ],
      [
        "Trivial"
      ]
    ]
  },
  {
    "args": [
      [
        [
          0,
          1,
          1,
          0,
          1,
          1,
          1,
          0,
          1,
          0
        ],
        [
          0,
          0,
          1,
          0,
          0,
          1,
          0,
          1,
          1,
          1
        ],
        [
          0,
          0,
          0,
          0,
          1,
          1,
          1,
          1,
          0,
          0
        ],
        [
          1,
          0,
          1,
          1,
          1,
          0,
          0,
          1,
          0,
          1
        ],
        [
          1,
          0,
          0,
          1,
          0,
          0,
          1,
          1,
          0,
          0
        ],
        [
          0,
          0,
          1,
          0,
          1,
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
          1,
          0,
          1,
          0,
          0,
          0,
          1
        ],
        [
          0,
          0,
          1,
          1,
          0,
          1,
          1,
          0,
          0,
          0
        ],
        [
          0,
          1,
          1,
          1,
          0,
          1,
          1,
          1,
          0,
          0
        ],
        [
          1,
          0,
          0,
          0,
          1,
          1,
          1,
          1,
          1,
          1
        ]
      ]
    ],
    "return": [
      [
        0,
        0,
        0,
        1,
        0,
        0,
        0,
        0,
        0,
        1
      ],
      [
        0,
        1,
        1,
        0,
        0,
        1,
        1,
        1,
        1,
        1
      ]
    ]
  }
]
```

## Credits

Found on Edabit: [Get the Diagonals](https://edabit.com/challenge/LQgpGFMK9t9MELvph)
