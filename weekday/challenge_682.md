# Challenge 682 - Farey Sequence

The Farey sequence of order `n` is the set of all fractions with a denominator between 1 and `n`, reduced and returned in ascending order. Given `n`, return the Farey sequence as a list, with each fraction being represented by a string in the form `"numerator/denominator"`.

## Examples
```python
farey(1) ➞ ["0/1", "1/1"]

farey(4) ➞ ["0/1", "1/4", "1/3", "1/2", "2/3", "3/4", "1/1"]

farey(5) ➞ ["0/1", "1/5", "1/4", "1/3", "2/5", "1/2", "3/5", "2/3", "3/4", "4/5", "1/1"]
```
## Notes

- The Farey sequence will always begin with `"0/1"` and end with `"1/1"`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def farey(n: int) -> list[str]:
    return []  # Put your code here!!!


test(682, farey)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            8
        ],
        "return": [
            "0/1",
            "1/8",
            "1/7",
            "1/6",
            "1/5",
            "1/4",
            "2/7",
            "1/3",
            "3/8",
            "2/5",
            "3/7",
            "1/2",
            "4/7",
            "3/5",
            "5/8",
            "2/3",
            "5/7",
            "3/4",
            "4/5",
            "5/6",
            "6/7",
            "7/8",
            "1/1"
        ]
    },
    {
        "args": [
            9
        ],
        "return": [
            "0/1",
            "1/9",
            "1/8",
            "1/7",
            "1/6",
            "1/5",
            "2/9",
            "1/4",
            "2/7",
            "1/3",
            "3/8",
            "2/5",
            "3/7",
            "4/9",
            "1/2",
            "5/9",
            "4/7",
            "3/5",
            "5/8",
            "2/3",
            "5/7",
            "3/4",
            "7/9",
            "4/5",
            "5/6",
            "6/7",
            "7/8",
            "8/9",
            "1/1"
        ]
    },
    {
        "args": [
            10
        ],
        "return": [
            "0/1",
            "1/10",
            "1/9",
            "1/8",
            "1/7",
            "1/6",
            "1/5",
            "2/9",
            "1/4",
            "2/7",
            "3/10",
            "1/3",
            "3/8",
            "2/5",
            "3/7",
            "4/9",
            "1/2",
            "5/9",
            "4/7",
            "3/5",
            "5/8",
            "2/3",
            "7/10",
            "5/7",
            "3/4",
            "7/9",
            "4/5",
            "5/6",
            "6/7",
            "7/8",
            "8/9",
            "9/10",
            "1/1"
        ]
    },
    {
        "args": [
            4
        ],
        "return": [
            "0/1",
            "1/4",
            "1/3",
            "1/2",
            "2/3",
            "3/4",
            "1/1"
        ]
    },
    {
        "args": [
            5
        ],
        "return": [
            "0/1",
            "1/5",
            "1/4",
            "1/3",
            "2/5",
            "1/2",
            "3/5",
            "2/3",
            "3/4",
            "4/5",
            "1/1"
        ]
    }
]
```
## Credits

Found on Edabit: [Farey Sequence](https://edabit.com/challenge/c6FoPFprcNW6u5oAn)
