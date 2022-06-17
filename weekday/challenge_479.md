# Challenge 479 - Return the Highest and Lowest Numbers

Create a function that accepts a string of space separated integers and returns the highest and lowest integers (as a string).

## Examples
```python
high_low("1 2 3 4 5") ➞ "5 1"

high_low("1 2 -3 4 5") ➞ "5 -3"

high_low("1 9 3 4 -5") ➞ "9 -5"

high_low("13") ➞ "13 13"
```
## Notes

- Output string must be two integers separated by a single space, and highest number is first.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def high_low(numbers: str) -> str:
    return ""  # Put your code here!!!


test(479, high_low)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "4 5 29 54 4 0 -214 542 -64 1 -3 6 -6"
        ],
        "return": "542 -214"
    },
    {
        "args": [
            "1 -1"
        ],
        "return": "1 -1"
    },
    {
        "args": [
            "1 1"
        ],
        "return": "1 1"
    },
    {
        "args": [
            "-1 -1"
        ],
        "return": "-1 -1"
    },
    {
        "args": [
            "1 -1 0"
        ],
        "return": "1 -1"
    },
    {
        "args": [
            "1 1 0"
        ],
        "return": "1 0"
    },
    {
        "args": [
            "-1 -1 0"
        ],
        "return": "0 -1"
    },
    {
        "args": [
            "42"
        ],
        "return": "42 42"
    }
]
```
## Credits

Found on Edabit: [Return the Highest and Lowest Numbers](https://edabit.com/challenge/K9w9hEd9Pn7DtMzjs)
