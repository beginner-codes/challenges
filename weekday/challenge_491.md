# Challenge 491 - One, Two, Skip a Few

Create a function which calculates how many numbers are missing from an ordered number line. This number line starts at the first value of the list, and increases by 1 to the end of the number line, ending at the last value of the list.
```python
how_many_missing([1, 2, 3, 8, 9]) ➞ 4

# The number line starts at 1 and ends at 9 (so the numbers 0 and 10 aren't missing from it).
# The numbers missing from this line are 4, 5, 6, and 7.
# 4 numbers are missing.
```
## Examples
```python
how_many_missing([1, 3]) ➞ 1

how_many_missing([7, 10, 11, 12]) ➞ 2

how_many_missing([1, 3, 5, 7, 9, 11]) ➞ 5

how_many_missing([5, 6, 7, 8]) ➞ 0
```
## Notes

- If the number line is complete, or the list is empty, return `0`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def how_many_missing(number_line: list[int]) -> int:
    return 0  # Put your code here!!!


test(491, how_many_missing)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                1,
                3
            ]
        ],
        "return": 1
    },
    {
        "args": [
            [
                7,
                10,
                11,
                12
            ]
        ],
        "return": 2
    },
    {
        "args": [
            [
                1,
                3,
                5,
                7,
                9,
                11
            ]
        ],
        "return": 5
    },
    {
        "args": [
            [
                5,
                6,
                7,
                8
            ]
        ],
        "return": 0
    },
    {
        "args": [
            [
                1,
                2,
                3,
                8,
                9
            ]
        ],
        "return": 4
    },
    {
        "args": [
            [
                1
            ]
        ],
        "return": 0
    },
    {
        "args": [
            []
        ],
        "return": 0
    }
]
```
## Credits

Found on Edabit: [One, Two, Skip a Few](https://edabit.com/challenge/Fw4fFSnTJfCsPBJ5u)
