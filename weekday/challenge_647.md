# Challenge 647 - Tweaking Letters

Create a function that tweaks letters by one forward (+1) or backwards (-1) according to a list.

## Examples
```python
tweak_letters("apple", [0, 1, -1, 0, -1]) ➞ "aqold"
# "p" + 1 => "q"; "p" - 1 => "o"; "e" - 1 => "d"

tweak_letters("many", [0, 0, 0, -1]) ➞ "manx"

tweak_letters("rhino", [1, 1, 1, 1, 1]) ➞ "sijop"
```
## Notes

- Don't worry about capital letters.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def tweak_letters(word: str, shift: list[int]) -> str:
    return ""  # Put your code here!!!


test(647, tweak_letters)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "xyz",
            [
                1,
                1,
                1
            ]
        ],
        "return": "yza"
    },
    {
        "args": [
            "apple",
            [
                0,
                1,
                -1,
                0,
                -1
            ]
        ],
        "return": "aqold"
    },
    {
        "args": [
            "many",
            [
                0,
                0,
                0,
                -1
            ]
        ],
        "return": "manx"
    },
    {
        "args": [
            "abc",
            [
                -1,
                -1,
                -1
            ]
        ],
        "return": "zab"
    },
    {
        "args": [
            "rhino",
            [
                1,
                1,
                1,
                1,
                1
            ]
        ],
        "return": "sijop"
    }
]
```
## Credits

Found on Edabit: [Tweaking Letters](https://edabit.com/challenge/QKyR63wENr4RMF9L7)
