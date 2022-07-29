# Challenge 507 - One Plus One

Create a function that outputs the result of a math expression given in words.

## Examples
```python
worded_math("One plus one") ➞ "Two"

worded_math("zero Plus one") ➞ "One"

worded_math("one minus one") ➞ "Zero"
```
## Notes

- Expect only the operations plus and minus.
- Expect to only get numbers and answers from `0` to `10`.
- The first letter of the answer must be capitalised.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def worded_math(math: str) -> str:
    return ""  # Put your code here!!!


test(507, worded_math)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "One plus one"
        ],
        "return": "Two"
    },
    {
        "args": [
            "zero Plus one"
        ],
        "return": "One"
    },
    {
        "args": [
            "one minus one"
        ],
        "return": "Zero"
    }
]
```
## Credits

Found on Edabit: [One Plus One](https://edabit.com/challenge/kzZD8Xp3EC7bipfxe)
