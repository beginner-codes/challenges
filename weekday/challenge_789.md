# Challenge 789 - Keyboard & Mouse

A keyboard and a mouse cost in total x, knowing that the keyboard costs y more than the mouse, calculate the price of the mouse.

## Examples
```python
mouse_cost({"Total": "$10.00", "Difference": "$0.40", "Mouse": "?"})
➞ {"Total": "$10.00", "Difference":"$0.40", "Mouse": "$4.8"}

mouse_cost({"Total": "$90.00", "Difference": "$5.40", "Mouse": "?"})
➞ {"Total": "$90.00", "Difference": "$5.40", "Mouse": "$42.3"}

mouse_cost({"Total": "$1.30", "Difference": "$0.80", "Mouse": "?"})
➞ {"Total": "$1.30", "Difference": "$0.80", "Mouse": "$0.25"}
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


def mouse_cost(data: dict[str, str]) -> dict[str, str]:
    return {}  # Put your code here!!!


test(789, mouse_cost)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            {
                "Total": "$3.90",
                "Difference": "$0.20",
                "Mouse": "?"
            }
        ],
        "return": {
            "Total": "$3.90",
            "Difference": "$0.20",
            "Mouse": "$1.85"
        }
    },
    {
        "args": [
            {
                "Total": "$1.90",
                "Difference": "$0.90",
                "Mouse": "?"
            }
        ],
        "return": {
            "Total": "$1.90",
            "Difference": "$0.90",
            "Mouse": "$0.5"
        }
    },
    {
        "args": [
            {
                "Total": "$1.30",
                "Difference": "$0.80",
                "Mouse": "?"
            }
        ],
        "return": {
            "Total": "$1.30",
            "Difference": "$0.80",
            "Mouse": "$0.25"
        }
    },
    {
        "args": [
            {
                "Total": "$20.00",
                "Difference": "$1.40",
                "Mouse": "?"
            }
        ],
        "return": {
            "Total": "$20.00",
            "Difference": "$1.40",
            "Mouse": "$9.3"
        }
    },
    {
        "args": [
            {
                "Total": "$0.801",
                "Difference": "$0.40",
                "Mouse": "?"
            }
        ],
        "return": {
            "Total": "$0.801",
            "Difference": "$0.40",
            "Mouse": "$0.2"
        }
    },
    {
        "args": [
            {
                "Total": "$10.00",
                "Difference": "$0.40",
                "Mouse": "?"
            }
        ],
        "return": {
            "Total": "$10.00",
            "Difference": "$0.40",
            "Mouse": "$4.8"
        }
    }
]
```

## Credits

Found on Edabit: [Key - Mouse (Logic)](https://edabit.com/challenge/vC7vwZdPAYqkcFH7J)
