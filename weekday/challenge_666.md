# Challenge 666 - Positives and Negatives

Create a function which validates that a list alternates between positive and negative numbers.

## Examples
```python
alternate_pos_neg([3, -2, 5, -5, 2, -8]) ➞ True

alternate_pos_neg([-6, 1, -1, 4, -3]) ➞ True

alternate_pos_neg([4, 4, -2, 3, -6, 10]) ➞ False
```
## Notes

- Lists can be of any length.
- It doesn't matter if a list begins/ends with a positive or negative, as long as it alternates.
- If a list contains 0, return `False` (as it is neither positive nor negative).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def alternate_pos_neg(numbers: list[int]) -> bool:
    return False  # Put your code here!!!


test(666, alternate_pos_neg)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                40
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                41,
                11,
                37,
                -30,
                -29,
                39,
                -45,
                15,
                -41,
                7
            ]
        ],
        "return": false
    },
    {
        "args": [
            [
                24,
                -10
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                3,
                -7,
                15,
                -18,
                0
            ]
        ],
        "return": false
    },
    {
        "args": [
            [
                -2,
                4,
                16,
                -15,
                24,
                2
            ]
        ],
        "return": false
    }
]

```
## Credits

Found on Edabit: [Positives and Negatives](https://edabit.com/challenge/HaxQfQTEpo7BFE5rz)
