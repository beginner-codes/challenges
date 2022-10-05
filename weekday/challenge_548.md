# Challenge 548 - Switcharoo

Create a function that takes a string and returns a new string with its first and last characters swapped, except under three conditions:

- If the length of the string is less than two, return `"Incompatible."`.
- If the argument is not a string, return `"Incompatible."`.
- If the first and last characters are the same, return `"Two's a pair."`.

## Examples
```python
flip_end_chars("Cat, dog, and mouse.") ➞ ".at, dog, and mouseC"

flip_end_chars("ada") ➞ "Two's a pair."

flip_end_chars("Ada") ➞ "adA"

flip_end_chars("z") ➞ "Incompatible."

flip_end_chars([1, 2, 3]) ➞ "Incompatible."
```
## Notes

- Tests are case-sensitive (e.g. `"A"` and `"a"` are not the same character).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test
from typing import Any, Literal, overload


@overload
def flip_end_chars(string: str) -> str:
    ...


@overload
def flip_end_chars(string: Any) -> Literal["Incompatible"] | str:
    ...


def flip_end_chars(string: str | Any) -> Literal["Incompatible"] | str:
    return "" # Put your code here!!!


test(548, flip_end_chars)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "#343473847#"
        ],
        "return": "Two's a pair."
    },
    {
        "args": [
            ""
        ],
        "return": "Incompatible."
    },
    {
        "args": [
            [
                1,
                2,
                3
            ]
        ],
        "return": "Incompatible."
    },
    {
        "args": [
            "dfdkf49824fdfdfjhd"
        ],
        "return": "Two's a pair."
    },
    {
        "args": [
            "Anna, Banana"
        ],
        "return": "anna, BananA"
    }
]
```
## Credits

Found on Edabit: [Switcharoo](https://edabit.com/challenge/tnKZCAkdnZpiuDiWA)
