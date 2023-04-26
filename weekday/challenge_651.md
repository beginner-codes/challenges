# Challenge 651 - Seven Boom!

Create a function that takes a list of numbers and return `"Boom!"` if the digit 7 appears in any of the numbers in the list. Otherwise, return `"there is no 7 in the list"`.

## Examples
```python
seven_boom([1, 2, 3, 4, 5, 6, 7]) ➞ "Boom!"
# 7 contains the number seven.

seven_boom([8, 6, 33, 100]) ➞ "there is no 7 in the list"
# None of the items contain 7 within them.

seven_boom([2, 55, 60, 97, 86]) ➞ "Boom!"
# 97 contains the number seven.
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def seven_boom(numbers: list[int]) -> str:
    return ""  # Put your code here!!!


test(651, seven_boom)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                86,
                48,
                100,
                66
            ]
        ],
        "return": "there is no 7 in the list"
    },
    {
        "args": [
            [
                76,
                55,
                44,
                32
            ]
        ],
        "return": "Boom!"
    },
    {
        "args": [
            [
                33,
                68,
                400,
                5
            ]
        ],
        "return": "there is no 7 in the list"
    },
    {
        "args": [
            [
                2,
                6,
                7,
                9,
                3
            ]
        ],
        "return": "Boom!"
    },
    {
        "args": [
            [
                35,
                4,
                9,
                37
            ]
        ],
        "return": "Boom!"
    }
]
```
## Credits

Found on Edabit: [Seven Boom!](https://edabit.com/challenge/BokhFunYBvsvHEjfx)
