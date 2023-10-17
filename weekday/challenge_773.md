# Challenge 773 - Grocery Store Prices

You are given a list of strings consisting of grocery items, with prices in parentheses. Return a list of prices in float format.

## Examples
```python
get_prices(["salad ($4.99)"]) ➞ [4.99]

get_prices([
  "artichokes ($1.99)",
  "rotiserrie chicken ($5.99)",
  "gum ($0.75)"
])

➞ [1.99, 5.99, 0.75]

get_prices([
  "ice cream ($5.99)",
  "banana ($0.20)",
  "sandwich ($8.50)",
  "soup ($1.99)"
])

➞ [5.99, 0.2, 8.50, 1.99]
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


def get_prices(products: list[str]) -> list[int]:
    return []  # Put your code here!!!


test(773, get_prices)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                "salad ($4.99)"
            ]
        ],
        "return": [
            4.99
        ]
    },
    {
        "args": [
            [
                "ice cream ($5.99)",
                "banana ($0.20)",
                "sandwich ($8.50)",
                "soup ($1.99)"
            ]
        ],
        "return": [
            5.99,
            0.2,
            8.5,
            1.99
        ]
    },
    {
        "args": [
            [
                "artichokes ($1.99)",
                "rotiserrie chicken ($5.99)",
                "gum ($0.75)"
            ]
        ],
        "return": [
            1.99,
            5.99,
            0.75
        ]
    },
    {
        "args": [
            [
                "pizza ($2.99)",
                "shampoo ($15.75)",
                "trash bags ($15.00)"
            ]
        ],
        "return": [
            2.99,
            15.75,
            15
        ]
    }
]
```

## Credits

Found on Edabit: [Grocery Store Prices](https://edabit.com/challenge/tQPApXhwoQ6zztxWJ)
