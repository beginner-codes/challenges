# Challenge 497 - Little Big Sequence

The number sequence is as follows:
```
5, 100, 6, 200, 7, 400, 8, 800, 9, 1600, 10, 3200, ...
```
Given that 5 is at position `1`, create a function that returns the number found at position `n` in the sequence.

## Examples
```python
little_big(4) ➞ 200

little_big(5) ➞ 7

little_big(28) ➞ 819200
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def little_big(n: int) -> int:
    return 0  # Put your code here!!!


test(497, little_big)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            1
        ],
        "return": 5
    },
    {
        "args": [
            2
        ],
        "return": 100
    },
    {
        "args": [
            3
        ],
        "return": 6
    },
    {
        "args": [
            4
        ],
        "return": 200
    },
    {
        "args": [
            5
        ],
        "return": 7
    },
    {
        "args": [
            6
        ],
        "return": 400
    },
    {
        "args": [
            7
        ],
        "return": 8
    },
    {
        "args": [
            8
        ],
        "return": 800
    },
    {
        "args": [
            9
        ],
        "return": 9
    },
    {
        "args": [
            30
        ],
        "return": 1638400
    }
]
```
## Credits

Found on Edabit: [Little Big Sequence](https://edabit.com/challenge/ecwE3tQK9Na8GJ9pN)
