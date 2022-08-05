# Challenge 512 - Explosion Intensity

Given a number, return a string of the word `"Boom"`, which varies in the following ways:

- The string should include `n` number of `"o"`s, unless `n` is below `2` (in that case, return `"boom"`).
- If `n` is evenly divisible by `2`, add an exclamation mark to the end.
- If `n` is evenly divisible by `5`, return the string in ALL CAPS.

The examples below should help clarify these instructions.

## Examples
```python
boom_intensity(4) ➞ "Boooom!"
# There are 4 "o"s and 4 is divisible by 2 (exclamation mark included)

boom_intensity(1) ➞ "boom"
# 1 is lower than 2, so we return "boom"

boom_intensity(5) ➞ "BOOOOOM"
# There are 5 "o"s and 5 is divisible by 5 (all caps)

boom_intensity(10) ➞ "BOOOOOOOOOOM!"
# There are 10 "o"s and 10 is divisible by 2 and 5 (all caps and exclamation mark included)
```
## Notes

- A number which is evenly divisible by `2` and `5` will have both effects applied.
- `"Boom"` will always start with a capital `"B"`, except when `n` is less than `2`, then return a minature explosion as `"boom"`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def boom_intensity(explosion: int) -> str:
    return ""  # Put your code here!!!


test(512, boom_intensity)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            0
        ],
        "return": "boom"
    },
    {
        "args": [
            1
        ],
        "return": "boom"
    },
    {
        "args": [
            2
        ],
        "return": "Boom!"
    },
    {
        "args": [
            3
        ],
        "return": "Booom"
    },
    {
        "args": [
            4
        ],
        "return": "Boooom!"
    },
    {
        "args": [
            5
        ],
        "return": "BOOOOOM"
    },
    {
        "args": [
            6
        ],
        "return": "Boooooom!"
    },
    {
        "args": [
            7
        ],
        "return": "Booooooom"
    },
    {
        "args": [
            8
        ],
        "return": "Boooooooom!"
    },
    {
        "args": [
            20
        ],
        "return": "BOOOOOOOOOOOOOOOOOOOOM!"
    },
    {
        "args": [
            50
        ],
        "return": "BOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOM!"
    }
]
```
## Credits

Found on Edabit: [Explosion Intensity](https://edabit.com/challenge/XYvyirQMkmPHGLaZi)
