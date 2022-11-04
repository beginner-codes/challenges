# Challenge 566 - Convert String to camelCase

Create a function that converts dash/underscore delimited words into camel casing. The first word within the output should be capitalized only if the original word was capitalized.

## Examples
```python
to_camel_case("A-B-C") ➞ "ABC"

to_camel_case("the-stealth-warrior") ➞ "theStealthWarrior"

to_camel_case("The_Stealth_Warrior") ➞ "TheStealthWarrior"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def to_camel_case(name: str) -> str:
    return "" # Put your code here!!!


test(566, to_camel_case)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "A-B-C"
        ],
        "return": "ABC"
    },
    {
        "args": [
            "The-Stealth-Warrior"
        ],
        "return": "TheStealthWarrior"
    },
    {
        "args": [
            "the_stealth_warrior"
        ],
        "return": "theStealthWarrior"
    },
    {
        "args": [
            ""
        ],
        "return": ""
    }
]
```
## Credits

Found on Edabit: [Convert String to camelCase](https://edabit.com/challenge/4bX7qAqELq9XJeB26)
