# Challenge 542 - Message from Space

You have received an encrypted message from space. Your task is to decrypt the message with the following simple rules:

- Message string will consist of capital letters, numbers, and brackets only.
- When there's a block of code inside the brackets, such as `[10AB]`, it means you need to repeat the letters `AB` for `10` times.
- Message can be embedded in multiple layers of blocks.
- Final decrypted message will only consist of capital letters.


Create a function that takes encrypted message txt and returns the decrypted message.

## Examples
```python
space_message("ABCD") ➞ "ABCD"

space_message("AB[3CD]") ➞ "ABCDCDCD"
# "AB" = "AB"
# "[3CD]" = "CDCDCD"

space_message("IF[2E]LG[5O]D") ➞ "IFEELGOOOOOD"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def space_message(encrypted: str) -> str:
    return "" # Put your code here!!!


test(542, space_message)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "AB[3CD]"
        ],
        "return": "ABCDCDCD"
    },
    {
        "args": [
            "ABCD"
        ],
        "return": "ABCD"
    },
    {
        "args": [
            "IF[2E]LG[5O]D"
        ],
        "return": "IFEELGOOOOOD"
    },
    {
        "args": [
            "MU[2B][2A][2S][2H][2I]RISN[4O]TAMA[4Z]ING"
        ],
        "return": "MUBBAASSHHIIRISNOOOOTAMAZZZZING"
    },
    {
        "args": [
            "AB[2C[2EF]G]"
        ],
        "return": "ABCEFEFGCEFEFG"
    },
    {
        "args": [
            "AB[2[3CD]]"
        ],
        "return": "ABCDCDCDCDCDCD"
    }
]
```
## Credits

Found on Edabit: [Message from Space](https://edabit.com/challenge/pkw5zmXmQ9qg9LYAi)
