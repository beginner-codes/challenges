# Challenge 462 - The Antipodes Average

In this challenge, you are given a list and in turn, you must obtain a smaller list, following three steps:

1. Split the list into two parts of equal length. If the given list has an odd length, then you have to eliminate the number in the middle of the list for obtaining two equal parts.
2. Sum each number of the first part with each number of the reversed second part, obtaining a new single list having the same length of the previous two.
3. Divide by two each number in the final list.

Given a list of integers, implement a function that returns a new list applying the above algorithm.

## Examples
```python
antipodes_average([1, 2, 3, 4]) ➞ [2.5, 2.5]
# Left part = [1, 2]
# Reversed right part = [4, 3]
# List resulting from the sum of each pair = [5, 5]
# Each number is divided by two = [2.5, 2.5]

antipodes_average([1, 2, 3, 4, 5]) ➞ [3, 3]
# The length of list is odd, number 3 (in the middle) is eliminated
# Left = [1, 2]
# Reversed right = [5, 4]
# Sum = [6, 6]
# Division by two = [3, 3]

antipodes_average([-1, -2]) ➞ [-1.5]
#  (-1 + -2) / 2 = [-1.5]
```
## Notes

- Every given list will contain at least two numbers.
- Into the given list, numbers will always be whole (either positives or negatives), but the numbers into the returned final list can also be a float.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from beginnercodes.challenges import test


def antipodes_average(numbers: list[int]) -> list[int]:
    return []  # Put your code here!!!


test(462, antipodes_average)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                1,
                2,
                3,
                4
            ]
        ],
        "return": [
            2.5,
            2.5
        ]
    },
    {
        "args": [
            [
                1,
                2,
                3,
                4,
                5
            ]
        ],
        "return": [
            3,
            3
        ]
    },
    {
        "args": [
            [
                -1,
                -2
            ]
        ],
        "return": [
            -1.5
        ]
    },
    {
        "args": [
            [
                1,
                2,
                5,
                10
            ]
        ],
        "return": [
            5.5,
            3.5
        ]
    },
    {
        "args": [
            [
                1,
                2,
                3,
                5,
                7,
                9
            ]
        ],
        "return": [
            5,
            4.5,
            4
        ]
    },
    {
        "args": [
            [
                -1,
                -4,
                -12,
                -2,
                -11,
                -6
            ]
        ],
        "return": [
            -3.5,
            -7.5,
            -7
        ]
    },
    {
        "args": [
            [
                5,
                -80,
                66,
                -8,
                -6
            ]
        ],
        "return": [
            -0.5,
            -44
        ]
    },
    {
        "args": [
            [
                -1,
                0,
                1
            ]
        ],
        "return": [
            0
        ]
    }
]
```
## Credits

Found on Edabit: [The Antipodes Average](https://edabit.com/challenge/oF8T7Apf7jfagC4fD)
