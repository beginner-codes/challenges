# Challenge 632 - Find the First Non-Repeated Character

Create a function that accepts a string as an argument and returns the first non-repeated character.

## Examples
```python
first_non_repeated_character("g") ➞ "g"

first_non_repeated_character("it was then the frothy word met the round night") ➞ "a"

first_non_repeated_character("the quick brown fox jumps then quickly blows air") ➞ "f"

first_non_repeated_character("hheelloo") ➞ False

first_non_repeated_character("") ➞ False
```
## Notes

- An empty string should return `False`.
- If every character repeats, return `False`.
- Don't worry about case sensitivity or non-alphanumeric characters.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def first_non_repeated_character(string: str) -> str | bool:
    return False  # Put your code here!!!


test(632, first_non_repeated_character)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "hheelloo"
        ],
        "return": false
    },
    {
        "args": [
            "the misty examination pleases into the drab county"
        ],
        "return": "x"
    },
    {
        "args": [
            ""
        ],
        "return": false
    },
    {
        "args": [
            "what if the brainy boss ate the afternoon"
        ],
        "return": "w"
    },
    {
        "args": [
            "the sympathetic mixture rejects into the leafy objective"
        ],
        "return": "p"
    }
]
```
## Credits

Found on Edabit: [Find the First Non-Repeated Character](https://edabit.com/challenge/mJB9CYyGsADLQPjnx)
