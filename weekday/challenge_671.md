# Challenge 671 - The Missing Link of an Arithmetic Progression

Your function will get a list with a number sequence. However, one item will be missing. It's your job to find out which one is not in the list.

To illustrate, given the list `[1, 3, 4, 5]`, 2 is missing so the output must be 2.

## Examples
```python
missing([1, 3, 4, 5]) ➞ 2

missing([2, 4, 6, 8, 10, 14, 16]) ➞ 12

missing([1.5, 2, 3]) ➞ 2.5
```
## Notes

- The missing item will never be the smallest or largest number in the list.
- In every list, exactly one item is missing.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def missing(sequence: list[int]) -> int:
    return 0  # Put your code here!!!


test(671, missing)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                1,
                19,
                28
            ]
        ],
        "return": 10
    },
    {
        "args": [
            [
                12,
                15,
                18,
                21,
                24,
                30,
                33
            ]
        ],
        "return": 27
    },
    {
        "args": [
            [
                0,
                60,
                180
            ]
        ],
        "return": 120
    },
    {
        "args": [
            [
                1,
                3,
                4,
                5
            ]
        ],
        "return": 2
    },
    {
        "args": [
            [
                2,
                4,
                6,
                8,
                10,
                14,
                16
            ]
        ],
        "return": 12
    }
]
```
## Credits

Found on Edabit: [The Missing Link of an Arithmetic Progression](https://edabit.com/challenge/xBPCwB8c4rYrGqY3v)
