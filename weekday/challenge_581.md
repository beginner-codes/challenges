# Challenge 581 - Secret Function 4.0

Create a function based on the input and output. Look at the examples, there is a pattern.

## Examples
```python
secret("p.one.two.three") ➞ "<p class='one two three'></p>"

secret("p.one") ➞ "<p class='one'></p>"

secret("p.four.five") ➞ "<p class='four five'></p>"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def secret(string: str) -> str:
    return ""  # Put your code here!!!


test(581, secret)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "p.four.five"
        ],
        "return": "<p class='four five'></p>"
    },
    {
        "args": [
            "p.one.two.three"
        ],
        "return": "<p class='one two three'></p>"
    },
    {
        "args": [
            "h3.one"
        ],
        "return": "<h3 class='one'></h3>"
    },
    {
        "args": [
            "h1.a.b.c.d"
        ],
        "return": "<h1 class='a b c d'></h1>"
    },
    {
        "args": [
            "p.one"
        ],
        "return": "<p class='one'></p>"
    }
]
```
## Credits

Found on Edabit: [Secret Function 4.0](https://edabit.com/challenge/arFpErP9oz36oTcXW)
