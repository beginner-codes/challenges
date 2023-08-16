# Challenge 728 - ABACABADABACABA

Create a function that follows the "ABACABADABACABA" rule up to a certain letter.

The abacabadabacaba pattern is created by starting with the first letter (a), and with each new letter you add place the existing string before and after.

For example:
```python
A ➞ **A**
B ➞ A**B**A
C ➞ ABA**C**ABA
D ➞ ABACABA**D**ABACABA
E ➞ ABACABADABACABA**E**ABACABADABACABA
F ➞ ABACABADABACABAEABACABADABACABA**F**ABACABADABACABAEABACABADABACABA

# And so on ...
```
## Examples
```python
aba("A") ➞ "A"

aba("B") ➞ "ABA"

aba("E") ➞ "ABACABADABACABAEABACABADABACABA"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def aba(letter: str) -> str:
    return ""  # Put your code here!!!


test(728, aba)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "C"
        ],
        "return": "ABACABA"
    },
    {
        "args": [
            "D"
        ],
        "return": "ABACABADABACABA"
    },
    {
        "args": [
            "G"
        ],
        "return": "ABACABADABACABAEABACABADABACABAFABACABADABACABAEABACABADABACABAGABACABADABACABAEABACABADABACABAFABACABADABACABAEABACABADABACABA"
    },
    {
        "args": [
            "A"
        ],
        "return": "A"
    },
    {
        "args": [
            "E"
        ],
        "return": "ABACABADABACABAEABACABADABACABA"
    }
]
```
## Credits

Found on Edabit: [ABACABADABACABA](https://edabit.com/challenge/4s9kNQFfk4D4Lbm4q)
