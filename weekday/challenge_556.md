# Challenge 556 - Changing a String into camelCase

Using Camel Case (or `camelCase`) is where the first word is in lower case, and all words after it have their first letter capitalised. Note that there are no spaces in between words!

Create a function that takes a string and returns it back in camelCase.

## Examples
```python
camelCasing("Hello World") ➞ "helloWorld"

camelCasing("snake_case") ➞ "snakeCase"

camelCasing("low high_HIGH") ➞ "lowHighHigh"
```
## Notes

- You need to remove all spaces and underscores.
- There will be no numbers in inputs.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def camelCasing(name: str) -> str:
    return "" # Put your code here!!!


test(556, camelCasing)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "unEcEsSARilY_loNG_vArIablE_NaME"
        ],
        "return": "unecessarilyLongVariableName"
    },
    {
        "args": [
            "low high_HIGH"
        ],
        "return": "lowHighHigh"
    },
    {
        "args": [
            "camel casing"
        ],
        "return": "camelCasing"
    },
    {
        "args": [
            "Hello World"
        ],
        "return": "helloWorld"
    },
    {
        "args": [
            "snake_case"
        ],
        "return": "snakeCase"
    }
]
```
## Credits

Found on Edabit: [Changing a String into camelCase](https://edabit.com/challenge/djLTSAc6h4bt6ehWu)
