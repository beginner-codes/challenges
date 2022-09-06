# Challenge 531 - Arrow Pattern 

Create a function that creates a pattern as a 2D list for a given number.

## Examples
```python
arrow(3) ➞ [
    ">",
    ">>",
    ">>>",
    ">>",
    ">"
]

arrow(4) ➞ [
    ">", 
    ">>", 
    ">>>", 
    ">>>>", 
    ">>>>",
    ">>>",
    ">>",
    ">"
]
```
## Notes

- Function argument will always be a number greater than 0.
- Odd numbers will have a single "peak".
- Even numbers have two "peaks".

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def arrow(size: int) -> list[str]:
    return [] # Put your code here!!!


test(531, arrow)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            7
        ],
        "return": [
            ">",
            ">>",
            ">>>",
            ">>>>",
            ">>>>>",
            ">>>>>>",
            ">>>>>>>",
            ">>>>>>",
            ">>>>>",
            ">>>>",
            ">>>",
            ">>",
            ">"
        ]
    },
    {
        "args": [
            3
        ],
        "return": [
            ">",
            ">>",
            ">>>",
            ">>",
            ">"
        ]
    },
    {
        "args": [
            9
        ],
        "return": [
            ">",
            ">>",
            ">>>",
            ">>>>",
            ">>>>>",
            ">>>>>>",
            ">>>>>>>",
            ">>>>>>>>",
            ">>>>>>>>>",
            ">>>>>>>>",
            ">>>>>>>",
            ">>>>>>",
            ">>>>>",
            ">>>>",
            ">>>",
            ">>",
            ">"
        ]
    },
    {
        "args": [
            10
        ],
        "return": [
            ">",
            ">>",
            ">>>",
            ">>>>",
            ">>>>>",
            ">>>>>>",
            ">>>>>>>",
            ">>>>>>>>",
            ">>>>>>>>>",
            ">>>>>>>>>>",
            ">>>>>>>>>>",
            ">>>>>>>>>",
            ">>>>>>>>",
            ">>>>>>>",
            ">>>>>>",
            ">>>>>",
            ">>>>",
            ">>>",
            ">>",
            ">"
        ]
    },
    {
        "args": [
            8
        ],
        "return": [
            ">",
            ">>",
            ">>>",
            ">>>>",
            ">>>>>",
            ">>>>>>",
            ">>>>>>>",
            ">>>>>>>>",
            ">>>>>>>>",
            ">>>>>>>",
            ">>>>>>",
            ">>>>>",
            ">>>>",
            ">>>",
            ">>",
            ">"
        ]
    },
    {
        "args": [
            4
        ],
        "return": [
            ">",
            ">>",
            ">>>",
            ">>>>",
            ">>>>",
            ">>>",
            ">>",
            ">"
        ]
    }
]
```
## Credits

Found on Edabit: [Arrow Pattern](https://edabit.com/challenge/BDcaZaqCuBCczeKZL)
