# Challenge 655 - Return the Sum of the Two Smallest Numbers

Create a function that takes a list of numbers and returns the sum of the two lowest positive numbers.

## Examples
```python
sum_two_smallest_nums([19, 5, 42, 2, 77]) ➞ 7

sum_two_smallest_nums([10, 343445353, 3453445, 3453545353453]) ➞ 3453455

sum_two_smallest_nums([2, 9, 6, -1]) ➞ 8

sum_two_smallest_nums([879, 953, 694, -847, 342, 221, -91, -723, 791, -587]) ➞ 563

sum_two_smallest_nums([3683, 2902, 3951, -475, 1617, -2385]) ➞ 4519
```
## Notes

- Don't count negative numbers.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def sum_two_smallest_nums(nums: list[int]) -> int:
    return 0  # Put your code here!!!


test(655, sum_two_smallest_nums)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                280,
                134,
                108
            ]
        ],
        "return": 242
    },
    {
        "args": [
            [
                280,
                134,
                108,
                1
            ]
        ],
        "return": 109
    },
    {
        "args": [
            [
                1,
                1,
                1,
                1
            ]
        ],
        "return": 2
    },
    {
        "args": [
            [
                19,
                5,
                42,
                2,
                77
            ]
        ],
        "return": 7
    },
    {
        "args": [
            [
                321,
                406,
                -176
            ]
        ],
        "return": 727
    }
]
```
## Credits

Found on Edabit: [Return the Sum of the Two Smallest Numbers](https://edabit.com/challenge/xYpG6ry6CLqgcwRWC)
