# Challenge 620 - Transform Upvotes

Create a function that transforms a string of upvote counts into a list of numbers. Each `k` represents a thousand.

## Examples
```python
transform_upvotes("6.8k 13.5k") ➞ [6800, 13500]

transform_upvotes("5.5k 8.9k 32") ➞ [5500, 8900, 32]

transform_upvotes("20.3k 3.8k 7.7k 992") ➞ [20300, 3800, 7700, 992]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def transform_upvotes(string: str) -> list[int]:
    return []  # Put your code here!!!


test(620, transform_upvotes)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "20.3k 3.8k 7.7k 992"
        ],
        "return": [
            20300,
            3800,
            7700,
            992
        ]
    },
    {
        "args": [
            "6.8k 13.5k"
        ],
        "return": [
            6800,
            13500
        ]
    },
    {
        "args": [
            "5.5k 8.9k 32"
        ],
        "return": [
            5500,
            8900,
            32
        ]
    }
]
```
## Credits

Found on Edabit: [Transform Upvotes](https://edabit.com/challenge/nT4y8naTzHgknsW6h)
