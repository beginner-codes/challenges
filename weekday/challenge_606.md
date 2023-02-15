# Challenge 606 - A Normal Sequence

Consider a sequence where the first two numbers are `0` and `1`, the next number of the sequence is the sum of the previous two numbers modulo three.

Create a function that finds the nth element of the sequence.

## Examples
```python
normal_sequence(1) ➞ 0

normal_sequence(2) ➞ 1

normal_sequence(3) ➞ 1
# (0+1)%3 = 1

normal_sequence(20) ➞ 2
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def normal_sequence(nth: int) -> int:
    return 0  # Put your code here!!!


test(606, normal_sequence)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            118
        ],
        "return": 2
    },
    {
        "args": [
            148
        ],
        "return": 2
    },
    {
        "args": [
            87
        ],
        "return": 2
    },
    {
        "args": [
            117
        ],
        "return": 0
    },
    {
        "args": [
            163
        ],
        "return": 1
    }
]
```
## Credits

Found on Edabit: [A Normal Sequence](https://edabit.com/challenge/9ED9zbHHhaPaBz2xi)
