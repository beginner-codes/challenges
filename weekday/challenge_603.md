# Challenge 603 - Mega Milestones

Given a number, return a string which contains varying amounts of the word `'MEGA'` depending on the given number's order of magnitude.

- If the number is less than 100, return `"not a mega milestone"`.
- Otherwise, start with the string `"MEGA milestone"`.
- For every order of magnitude over 100 that the number is, add the word `"MEGA"` to the start of the string.

See the examples below for further clarification!

## Examples
```python
how_mega_is_it(54) ➞ "not a mega milestone"

how_mega_is_it(143) ➞ "MEGA milestone"

how_mega_is_it(1000) ➞ "MEGA MEGA milestone"

how_mega_is_it(9999.9) ➞ "MEGA MEGA milestone"

how_mega_is_it(10000) ➞ "MEGA MEGA MEGA milestone"
```
## Notes

- Large negative numbers can also be considered as MEGA, so use the absolute values.
- You can expect decimal numbers as well as whole numbers.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def how_mega_is_it(number: int) -> str:
    return ""  # Put your code here!!!


test(603, how_mega_is_it)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            387482
        ],
        "return": "MEGA MEGA MEGA MEGA milestone"
    },
    {
        "args": [
            9999.9
        ],
        "return": "MEGA MEGA milestone"
    },
    {
        "args": [
            54
        ],
        "return": "not a mega milestone"
    },
    {
        "args": [
            143
        ],
        "return": "MEGA milestone"
    },
    {
        "args": [
            10000
        ],
        "return": "MEGA MEGA MEGA milestone"
    }
]
```
## Credits

Found on Edabit: [Mega Milestones](https://edabit.com/challenge/n3zH5NvzPXb2qd5N5)
