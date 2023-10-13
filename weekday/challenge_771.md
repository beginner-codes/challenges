# Challenge 771 - The Sweetest Ice Cream

Create a function which takes a list of dictionaries representing icecream flavors and returns the sweetness value of the sweetest ice cream.

Each icecream dictionary has the following structure:
```json
{
  "flavor": "Vanilla",
  "num_sprinkles": 0
}
```

Each sprinkle has a sweetness value of 1 and each flavor has a sweetness value found in this table:
```
Flavors         Sweetness Value
Plain           0
Vanilla         5
ChocolateChip   5
Strawberry      10
Chocolate       10
```
## Examples
```python
sweetest_icecream(
    [
        {
            "flavor": "Strawberry",
            "num_sprinkles": 0
        },
        {
            "flavor": "Plain",
            "num_sprinkles": 18
        }
    ]
) ➞ 18

sweetest_icecream(
    [
        {
            "flavor": "Chocolate",
            "num_sprinkles": 23
        },
        {
            "flavor": "Chocolate",
            "num_sprinkles": 23
        }
    ]
) ➞ 33

sweetest_icecream(
    [
        {
            "flavor": "Plain",
            "num_sprinkles": 18
        },
        {
            "flavor": "Plain",
            "num_sprinkles": 34
        },
        {
            "flavor": "Plain",
            "num_sprinkles": 81
        }
    ]
) ➞ 81
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
from typing import TypedDict
from beginnercodes.challenges import test


class Icecream(TypedDict):
    flavor: str
    num_sprinkles: int


def sweetest_icecream(icecreams: list[Icecream]) -> int:
    return 0  # Put your code here!!!


test(771, sweetest_icecream)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                {
                    "flavor": "Vanilla",
                    "num_sprinkles": 12
                },
                {
                    "flavor": "Strawberry",
                    "num_sprinkles": 7
                }
            ]
        ],
        "return": 17
    },
    {
        "args": [
            [
                {
                    "flavor": "Strawberry",
                    "num_sprinkles": 7
                },
                {
                    "flavor": "Vanilla",
                    "num_sprinkles": 12
                },
                {
                    "flavor": "Chocolate",
                    "num_sprinkles": 13
                }
            ]
        ],
        "return": 23
    },
    {
        "args": [
            [
                {
                    "flavor": "Vanilla",
                    "num_sprinkles": 12
                },
                {
                    "flavor": "Chocolate",
                    "num_sprinkles": 23
                },
                {
                    "flavor": "Plain",
                    "num_sprinkles": 18
                },
                {
                    "flavor": "Chocolate",
                    "num_sprinkles": 13
                },
                {
                    "flavor": "Strawberry",
                    "num_sprinkles": 0
                },
                {
                    "flavor": "Plain",
                    "num_sprinkles": 34
                },
                {
                    "flavor": "Chocolate",
                    "num_sprinkles": 23
                }
            ]
        ],
        "return": 34
    },
    {
        "args": [
            [
                {
                    "flavor": "Strawberry",
                    "num_sprinkles": 0
                },
                {
                    "flavor": "Vanilla",
                    "num_sprinkles": 12
                },
                {
                    "flavor": "Chocolate",
                    "num_sprinkles": 13
                },
                {
                    "flavor": "Chocolate",
                    "num_sprinkles": 23
                },
                {
                    "flavor": "Plain",
                    "num_sprinkles": 34
                },
                {
                    "flavor": "Vanilla",
                    "num_sprinkles": 12
                },
                {
                    "flavor": "Vanilla",
                    "num_sprinkles": 0
                },
                {
                    "flavor": "Vanilla",
                    "num_sprinkles": 0
                }
            ]
        ],
        "return": 34
    },
    {
        "args": [
            [
                {
                    "flavor": "Plain",
                    "num_sprinkles": 34
                },
                {
                    "flavor": "Vanilla",
                    "num_sprinkles": 0
                },
                {
                    "flavor": "Vanilla",
                    "num_sprinkles": 0
                },
                {
                    "flavor": "Vanilla",
                    "num_sprinkles": 0
                },
                {
                    "flavor": "Plain",
                    "num_sprinkles": 18
                },
                {
                    "flavor": "Plain",
                    "num_sprinkles": 34
                }
            ]
        ],
        "return": 34
    }
]
```

## Credits

Found on Edabit: [The Sweetest Ice Cream](https://edabit.com/challenge/uerTkWm9K3oMtMZKz)
