# Challenge 683 - Consecutive Numbers

Given a list of random digits of any length, return True if a given number appears a given number of times in a row, False otherwise.

## Worked Example
```python
is_there_consecutive([1, 3, 5, 5, 3, 3, 1], 3, 2) ➞ True
# Second parameter is the number to look out for (3).
# Third parameter means you need to find the number 3 twice in a row.
# Return True if it can be found.
```
## Examples
```python
is_there_consecutive([1, 2, 3, 4, 5], 1, 1) ➞ True

is_there_consecutive([3], 1, 0) ➞ True

is_there_consecutive([2, 2, 3, 2, 2, 2, 2, 3, 4, 1, 5], 3, 2) ➞ False

is_there_consecutive([5, 5, 5, 5, 5], 5, 7) ➞ False
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def is_there_consecutive(numbers: list[int], number: int, repeats: int) -> bool:
    return False  # Put your code here!!!


test(683, is_there_consecutive)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                1,
                3,
                5,
                5,
                3,
                3,
                1
            ],
            3,
            2
        ],
        "return": true
    },
    {
        "args": [
            [
                1,
                2,
                3,
                4,
                5
            ],
            1,
            1
        ],
        "return": true
    },
    {
        "args": [
            [
                3
            ],
            1,
            0
        ],
        "return": true
    },
    {
        "args": [
            [
                2,
                2,
                2,
                2,
                2,
                2,
                3,
                4,
                1,
                5
            ],
            3,
            2
        ],
        "return": false
    },
    {
        "args": [
            [
                1,
                1,
                2,
                2,
                3,
                3,
                4,
                4,
                5,
                5,
                6,
                6,
                7,
                7,
                8,
                8,
                9,
                9,
                0,
                0
            ],
            5,
            2
        ],
        "return": true
    }
]
```
## Credits

Found on Edabit: [Consecutive Numbers](https://edabit.com/challenge/2Tr4gAzWimWvGpJW7)
