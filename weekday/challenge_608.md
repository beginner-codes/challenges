# Challenge 608 - Money Formatting

Given a number, return a string which is formatted into US Dollars and cents!

Remember that:

- You should round to two digits after the decimal point (even for integers).
- Thousandths should be separated by commas.

## Examples
```python
dolla_dolla_bills(10) ➞ "$10.00"

dolla_dolla_bills(1000000) ➞ "$1,000,000.00"

dolla_dolla_bills(-314159.2653) ➞ "-$314,159.27"

dolla_dolla_bills(-56.99) ➞ "-$56.99"
```
## Notes

- There will be both negative and positive inputs.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def dolla_dolla_bills(number: int) -> str:
    return ""  # Put your code here!!!


test(608, dolla_dolla_bills)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            0.05
        ],
        "return": "$0.05"
    },
    {
        "args": [
            -0.008
        ],
        "return": "-$0.01"
    },
    {
        "args": [
            31.4159
        ],
        "return": "$31.42"
    },
    {
        "args": [
            10
        ],
        "return": "$10.00"
    },
    {
        "args": [
            -314159.2653
        ],
        "return": "-$314,159.27"
    }
]
```
## Credits

Found on Edabit: [Money Formatting](https://edabit.com/challenge/eKJ8E6wnd9GMWxGaZ)
