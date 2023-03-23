# Challenge 628 - Capitalize the First Letter of Each Word

Create a function that takes a string as an argument and converts the first character of each word to uppercase. Return the newly formatted string.

## Examples
```python
make_title("This is a title") ➞ "This Is A Title"

make_title("capitalize every word") ➞ "Capitalize Every Word"

make_title("I Like Pizza") ➞ "I Like Pizza"

make_title("PIZZA PIZZA PIZZA") ➞ "PIZZA PIZZA PIZZA"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def make_title(string: str) -> str:
    return ""  # Put your code here!!!


test(628, make_title)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "Don't count your ChiCKens BeFore They HatCh"
        ],
        "return": "Don't Count Your ChiCKens BeFore They HatCh"
    },
    {
        "args": [
            "i aM a tITLE"
        ],
        "return": "I AM A TITLE"
    },
    {
        "args": [
            "PIZZA PIZZA PIZZA"
        ],
        "return": "PIZZA PIZZA PIZZA"
    },
    {
        "args": [
            "I Like Pizza"
        ],
        "return": "I Like Pizza"
    },
    {
        "args": [
            "I AM A TITLE"
        ],
        "return": "I AM A TITLE"
    }
]

```
## Credits

Found on Edabit: [Capitalize the First Letter of Each Word](https://edabit.com/challenge/hxr3ZyPw2bZzrHEsf)
