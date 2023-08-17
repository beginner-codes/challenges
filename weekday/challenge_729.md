# Challenge 729 - Convert camelCase to snake_case

Create a function that takes a string of words (or just one word) and converts each word from camelCase to snake_case.

## Examples
```python
camel_to_snake("magicCarrots") ➞ "magic_carrots"

camel_to_snake("greatApples for aSmellyRhino") ➞ "great_apples for a_smelly_rhino"

camel_to_snake("thatsGreat") ➞ "thats_great"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def camel_to_snake(string: str) -> str:
    return ""  # Put your code here!!!


test(729, camel_to_snake)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "magicCarrots"
        ],
        "return": "magic_carrots"
    },
    {
        "args": [
            "greatApples for aSmellyRhino"
        ],
        "return": "great_apples for a_smelly_rhino"
    },
    {
        "args": [
            "th1sSh0uldB3FineT00"
        ],
        "return": "th1s_sh0uld_b3_fine_t00"
    }
]
```
## Credits

Found on Edabit: [Convert camelCase to snake_case](https://edabit.com/challenge/TCQkKzgi8FFYYG4kR)
