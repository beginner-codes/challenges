# Challenge 619 - Partially Hidden String

Create a function that takes a phrase and transforms each word using the following rules:

- Keep first and last character the same.
- Transform middle characters into dashes `-`.

## Examples
```python
partially_hide("skies were pretty") ➞ "s---s w--e p----y"

partially_hide("red is not my color") ➞ "r-d is n-t my c---r"

partially_hide("She rolled her eyes") ➞ "S-e r----d h-r e--s"

partially_hide("Harry went to fight the basilisk") ➞ "H---y w--t to f---t t-e b------k"
```
## Notes

- Words with two or fewer letters should not be hidden at all.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def partially_hide(string: str) -> str:
    return ""  # Put your code here!!!


test(619, partially_hide)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "skies were so beautiful"
        ],
        "return": "s---s w--e so b-------l"
    },
    {
        "args": [
            "so many options"
        ],
        "return": "so m--y o-----s"
    },
    {
        "args": [
            "Harry went to fight the basilisk"
        ],
        "return": "H---y w--t to f---t t-e b------k"
    },
    {
        "args": [
            "the orient express"
        ],
        "return": "t-e o----t e-----s"
    },
    {
        "args": [
            "She rolled her eyes"
        ],
        "return": "S-e r----d h-r e--s"
    }
]
```
## Credits

Found on Edabit: [Partially Hidden String](https://edabit.com/challenge/h9hp2vGKbHJBzN87i)
