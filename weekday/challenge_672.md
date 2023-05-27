# Challenge 672 - Complete the Word

An input string can be completed if additional letters can be added and no letters need to be taken away to match the word. Furthermore, the order of the letters in the input string must be the same as the order of letters in the final word.

Create a function that, given an input string, determines if the word can be completed.

## Examples
```python
can_complete("butl", "beautiful") ➞ True
# We can add "ea" between "b" and "u", and "ifu" between "t" and "l".

can_complete("butlz", "beautiful") ➞ False
# "z" does not exist in the word beautiful.

can_complete("tulb", "beautiful") ➞ False
# Although "t", "u", "l" and "b" all exist in "beautiful", they are incorrectly ordered.

can_complete("bbutl", "beautiful") ➞ False
# Too many "b"s, beautiful has only 1.
```
## Notes

- Both string input and word are lowercase.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def can_complete(initial: str, word: str) -> bool:
    return False  # Put your code here!!!


test(672, can_complete)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "bbutl",
            "beautiful"
        ],
        "return": false
    },
    {
        "args": [
            "tulb",
            "beautiful"
        ],
        "return": false
    },
    {
        "args": [
            "sgi",
            "something"
        ],
        "return": false
    },
    {
        "args": [
            "butl",
            "beautiful"
        ],
        "return": true
    },
    {
        "args": [
            "sg",
            "something"
        ],
        "return": true
    }
]
```
## Credits

Found on Edabit: [Complete the Word](https://edabit.com/challenge/bd2fLqAxHfGTx86Qx)
