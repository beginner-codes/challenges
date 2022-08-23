# Challenge 524 - First N Mid 

Create a function that takes a string and returns the first character of every word if the length of the word is even and the middle character if the length of the word is odd.

## Examples
```python
stmid("Alexa have to paid") ➞ "ehtp"
# "e" is the middle character of "Alexa"
# "h" is the first character of "have"

stmid("Th3 0n3 4nd 0n1y") ➞ "hnn0"

stmid("who is the winner") ➞ "hihw"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def stmid(words: str) -> str:
    return "" # Put your code here!!!


test(524, stmid)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "who is the winner"
        ],
        "return": "hihw"
    },
    {
        "args": [
            "Th3 0n3 4nd 0n1y"
        ],
        "return": "hnn0"
    },
    {
        "args": [
            "Alexa have to paid"
        ],
        "return": "ehtp"
    }
]
```
## Credits

Found on Edabit: [First N Mid](https://edabit.com/challenge/fYMjhe7BnijXwfNpF)
