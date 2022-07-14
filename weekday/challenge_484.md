# Challenge 484 - Loves Me, Loves Me Not...

"Loves me, loves me not" is a traditional game in which a person plucks off all the petals of a flower one by one, saying the phrase "Loves me" and "Loves me not" when determining whether the one that they love, loves them back.

Given a number of petals, return a string which repeats the phrases `"Loves me"` and `"Loves me not"` for every alternating petal, and return the last phrase in all caps. *Remember to put a comma and space between phrases.*

## Examples
```python
loves_me(3) ➞ "Loves me, Loves me not, LOVES ME"

loves_me(6) ➞ "Loves me, Loves me not, Loves me, Loves me not, Loves me, LOVES ME NOT"

loves_me(1) ➞ "LOVES ME"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def loves_me(petals: int) -> str:
    return ""  # Put your code here!!!


test(484, loves_me)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            1
        ],
        "return": "LOVES ME"
    },
    {
        "args": [
            2
        ],
        "return": "Loves me, LOVES ME NOT"
    },
    {
        "args": [
            3
        ],
        "return": "Loves me, Loves me not, LOVES ME"
    },
    {
        "args": [
            4
        ],
        "return": "Loves me, Loves me not, Loves me, LOVES ME NOT"
    },
    {
        "args": [
            5
        ],
        "return": "Loves me, Loves me not, Loves me, Loves me not, LOVES ME"
    },
    {
        "args": [
            6
        ],
        "return": "Loves me, Loves me not, Loves me, Loves me not, Loves me, LOVES ME NOT"
    },
    {
        "args": [
            7
        ],
        "return": "Loves me, Loves me not, Loves me, Loves me not, Loves me, Loves me not, LOVES ME"
    },
    {
        "args": [
            8
        ],
        "return": "Loves me, Loves me not, Loves me, Loves me not, Loves me, Loves me not, Loves me, LOVES ME NOT"
    },
    {
        "args": [
            9
        ],
        "return": "Loves me, Loves me not, Loves me, Loves me not, Loves me, Loves me not, Loves me, Loves me not, LOVES ME"
    },
    {
        "args": [
            10
        ],
        "return": "Loves me, Loves me not, Loves me, Loves me not, Loves me, Loves me not, Loves me, Loves me not, Loves me, LOVES ME NOT"
    }
]
```
## Credits

Found on Edabit: [Loves Me, Loves Me Not...](https://edabit.com/challenge/6pEGXsuCAxbWTRkgc)
