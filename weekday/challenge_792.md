# Challenge 792 - Word to Bitstring to Boolean List

Create a function that converts a word to a bitstring and then to a boolean list based on the following criteria:

- Locate the position of the letter in the English alphabet (from 1 to 26).
- Odd positions will be represented as 1 and even positions will be represented as 0.
- Convert the represented positions to boolean values, 1 for True and 0 for False.

Store the conversions into an array.

## Examples
```python
to_boolean_list("deep") ➞ [False, True, True, False]
# deep converts to 0110
# d is the 4th alphabet - 0
# e is the 5th alphabet - 1
# e is the 5th alphabet - 1
# p is the 16th alphabet - 0

to_boolean_list("loves") ➞ [False, True, False, True, True]

to_boolean_list("tesh") ➞ [False, True, True, False]
```
## Notes

- The letter `A` is at position 1 and `Z` at 26
- All input strings are in lowercase letters of the English alphabet

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. *
*[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a
key `args` that are a list of parameters your function should take. The `return` key is what your function should return
given the `args`.

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your
solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:

```python
from __future__ import annotations
from beginnercodes.challenges import test


def to_boolean_list(word: str) -> list[bool]:
    return []  # Put your code here!!!


test(792, to_boolean_list)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            "loves"
        ],
        "return": [
            false,
            true,
            false,
            true,
            true
        ]
    },
    {
        "args": [
            "exotic"
        ],
        "return": [
            true,
            false,
            true,
            false,
            true,
            true
        ]
    },
    {
        "args": [
            "tesh"
        ],
        "return": [
            false,
            true,
            true,
            false
        ]
    },
    {
        "args": [
            "exquisite"
        ],
        "return": [
            true,
            false,
            true,
            true,
            true,
            true,
            true,
            false,
            true
        ]
    },
    {
        "args": [
            "tesha"
        ],
        "return": [
            false,
            true,
            true,
            false,
            true
        ]
    }
]

```

## Credits

Found on Edabit: [Word to Bitstring to Boolean List](https://edabit.com/challenge/temD7SmTyhdmME75i)
