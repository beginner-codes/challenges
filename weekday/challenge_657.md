# Challenge 657 - Natural Emptiness

In abstract set theory, a construction due to von Neumann represents the natural numbers by sets, as follows:
```
0 = [ ] is the empty set
1 = 0 ∪ [ 0 ] = [ 0 ] = [ [ ] ]
2 = 1 ∪ [ 1 ] = [ 0, 1 ] = [ [ ], [ [ ] ] ]
n = n−1 ∪ [ n−1 ] = ...
```
Write a function that receives an integer and produces the representing set.

## Examples
```python
rep_set(0) ➞ []

rep_set(1) ➞ [[]]

rep_set(2) ➞ [[], [[]]]

rep_set(3) ➞ [[], [[]], [[], [[ ]]]]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def rep_set(values: int) -> list[list]:
    return []  # Put your code here!!!


test(657, rep_set)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            0
        ],
        "return": []
    },
    {
        "args": [
            2
        ],
        "return": [
            [],
            [
                []
            ]
        ]
    },
    {
        "args": [
            3
        ],
        "return": [
            [],
            [
                []
            ],
            [
                [],
                [
                    []
                ]
            ]
        ]
    },
    {
        "args": [
            1
        ],
        "return": [
            []
        ]
    }
]
```
## Credits

Found on Edabit: [Natural Emptiness](https://edabit.com/challenge/w4fikTnBs8zhuLRY4)
