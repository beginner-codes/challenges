# Challenge 611 - The Perrin Sequence


Each number in the Perrin sequence is created by summing the numbers two positions and three positions before it. The first three numbers are `(3, 0, 2)`, and the sequence is extended as follows:
```
P(0) P(1) P(2) P(3) P(4) P(5) P(6) P(7) ... P(n)
3,   0,   2,   3,   2,   5,   5,   7,   ... ?
```
Given a value for `n`, return the Perrin number `P(n)`.

## Examples
```python
perrin(1) ➞ 0

perrin(8) ➞ 10

perrin(26) ➞ 1497
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def perrin(n: int) -> int:
    return 0  # Put your code here!!!


test(611, perrin)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            27
        ],
        "return": 1983
    },
    {
        "args": [
            46
        ],
        "return": 414646
    },
    {
        "args": [
            52
        ],
        "return": 2240877
    },
    {
        "args": [
            50
        ],
        "return": 1276942
    },
    {
        "args": [
            41
        ],
        "return": 101639
    }
]
```
## Credits

Found on Edabit: [The Perrin Sequence](https://edabit.com/challenge/MfypAQedEAun4oQFA)
