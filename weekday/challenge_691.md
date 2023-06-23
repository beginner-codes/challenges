# Challenge 691 - Product of All Other Numbers

You have a list of integers, and for each index you want to find the product of every integer except the integer at that index.

Create a function that takes a list of integers and returns a list of the products.

## Examples
```python
get_products([1, 7, 3, 4]) ➞ [84, 12, 28, 21]

get_products([1, 2, 6, 5, 9]) ➞ [540, 270, 90, 108, 60]

get_products([1, 2, 3, 0, 5]) ➞ [0, 0, 0, 30, 0]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def get_products(numbers: list[int]) -> list[int]:
    return []  # Put your code here!!!


test(691, get_products)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                1,
                7,
                3,
                4
            ]
        ],
        "return": [
            84,
            12,
            28,
            21
        ]
    },
    {
        "args": [
            [
                1,
                2,
                6,
                5,
                9
            ]
        ],
        "return": [
            540,
            270,
            90,
            108,
            60
        ]
    },
    {
        "args": [
            [
                1,
                2,
                3,
                0,
                5
            ]
        ],
        "return": [
            0,
            0,
            0,
            30,
            0
        ]
    }
]
```
## Credits

Found on Edabit: [Product of All Other Numbers](https://edabit.com/challenge/dsAPLuCpkKCBELk24)
