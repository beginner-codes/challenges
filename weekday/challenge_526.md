# Challenge 526 - Expand a Number 

Create a function that expands a number into a string as shown below:
```python
25 ➞ "20 + 5"
70701 ➞ "70000 + 700 + 1"
685 ➞ "600 + 80 + 5"
```
## Examples
```python
expanded_form(70304) ➞ "70000 + 300 + 4"

expanded_form(1037903) ➞ "1000000 + 30000 + 7000 + 900 + 3"

expanded_form(802539) ➞ "800000 + 2000 + 500 + 30 + 9"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def expanded_form(number: int) -> str:
    return "" # Put your code here!!!


test(526, expanded_form)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            2070504
        ],
        "return": "2000000 + 70000 + 500 + 4"
    },
    {
        "args": [
            5030708
        ],
        "return": "5000000 + 30000 + 700 + 8"
    },
    {
        "args": [
            2736692
        ],
        "return": "2000000 + 700000 + 30000 + 6000 + 600 + 90 + 2"
    },
    {
        "args": [
            3307098
        ],
        "return": "3000000 + 300000 + 7000 + 90 + 8"
    },
    {
        "args": [
            12
        ],
        "return": "10 + 2"
    },
    {
        "args": [
            607805
        ],
        "return": "600000 + 7000 + 800 + 5"
    },
    {
        "args": [
            1037903
        ],
        "return": "1000000 + 30000 + 7000 + 900 + 3"
    },
    {
        "args": [
            70903
        ],
        "return": "70000 + 900 + 3"
    },
    {
        "args": [
            2900837
        ],
        "return": "2000000 + 900000 + 800 + 30 + 7"
    },
    {
        "args": [
            42
        ],
        "return": "40 + 2"
    }
]
```
## Credits

Found on Edabit: [Expand a Number I](https://edabit.com/challenge/SQo9Jx5ih2iHG8JAn)
