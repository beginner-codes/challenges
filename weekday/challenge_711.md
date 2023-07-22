# Challenge 711 - Simplified Fractions

Create a function that returns the simplified version of a fraction.

## Examples
```python
simplify("4/6") ➞ "2/3"

simplify("10/11") ➞ "10/11"

simplify("100/400") ➞ "1/4"

simplify("8/4") ➞ "2"
```
## Notes

- A fraction is simplified if there are no common factors (except 1) between the numerator and the denominator. For example, `4/6` is not simplified, since `4` and `6` both share `2` as a factor.
- If improper fractions can be transformed into integers, do so in your code. 

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def simplify(fraction: str) -> str:
    return ""  # Put your code here!!!


test(711, simplify)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "7/4"
        ],
        "return": "7/4"
    },
    {
        "args": [
            "50/25"
        ],
        "return": "2"
    },
    {
        "args": [
            "5/7"
        ],
        "return": "5/7"
    },
    {
        "args": [
            "5/45"
        ],
        "return": "1/9"
    },
    {
        "args": [
            "6/4"
        ],
        "return": "3/2"
    }
]
```
## Credits

Found on Edabit: [Simplified Fractions](https://edabit.com/challenge/vQgmyjcjMoMu9YGGW)
