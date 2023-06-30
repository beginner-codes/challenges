# Challenge 696 - Number of Even or Odd Digits

Create a function that takes in a list of integers and returns the number of even or odd digits for each number, depending on the parameter.

## Examples
```python
count_digits([22, 53, 99, 61, 777, 8], "odd") ➞ [0, 2, 2, 1, 3, 0]

count_digits([22, 53, 99, 61, 777, 8], "even") ➞ [2, 0, 0, 1, 0, 1]

count_digits([54, 113, 89, 10], "odd") ➞ [1, 3, 1, 1]

count_digits([54, 113, 89, 10], "even") ➞ [1, 0, 1, 1]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def count_digits(numbers: list[int], t: str) -> list[int]:
    return []  # Put your code here!!!


test(696, count_digits)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                22,
                53,
                99,
                61,
                777,
                8
            ],
            "odd"
        ],
        "return": [
            0,
            2,
            2,
            1,
            3,
            0
        ]
    },
    {
        "args": [
            [
                54,
                113,
                89,
                10
            ],
            "even"
        ],
        "return": [
            1,
            0,
            1,
            1
        ]
    },
    {
        "args": [
            [
                17,
                19,
                21
            ],
            "odd"
        ],
        "return": [
            2,
            2,
            1
        ]
    },
    {
        "args": [
            [
                54,
                113,
                89,
                10
            ],
            "odd"
        ],
        "return": [
            1,
            3,
            1,
            1
        ]
    },
    {
        "args": [
            [
                22,
                53,
                99,
                61,
                777,
                8
            ],
            "even"
        ],
        "return": [
            2,
            0,
            0,
            1,
            0,
            1
        ]
    }
]
```
## Credits

Found on Edabit: [Number of Even or Odd Digits](https://edabit.com/challenge/gdzS7pXsPexY8j4A3)
