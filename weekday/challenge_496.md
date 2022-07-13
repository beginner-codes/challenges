# Challenge 496 - Odds vs. Evens

Given an integer, return `"odd"` if the sum of all odd digits is greater than the sum of all even digits. Return `"even"` if the sum of even digits is greater than the sum of odd digits, and `"equal"` if both sums are the same.

## Examples
```python
odds_vs_evens(97428) ➞ "odd"
# odd = 16 (9+7)
# even = 14 (4+2+8)

odds_vs_evens(81961) ➞ "even"
# odd = 11 (1+9+1)
# even = 14 (8+6)

odds_vs_evens(54870) ➞ "equal"
# odd = 12 (5+7)
# even = 12 (4+8+0)
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def odds_vs_evens(number: int) -> str:
    return ""  # Put your code here!!!


test(496, odds_vs_evens)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            44547
        ],
        "return": "equal"
    },
    {
        "args": [
            412420
        ],
        "return": "even"
    },
    {
        "args": [
            128797
        ],
        "return": "odd"
    },
    {
        "args": [
            838768
        ],
        "return": "even"
    },
    {
        "args": [
            371910
        ],
        "return": "odd"
    },
    {
        "args": [
            769431
        ],
        "return": "odd"
    },
    {
        "args": [
            221294
        ],
        "return": "equal"
    },
    {
        "args": [
            859307
        ],
        "return": "odd"
    },
    {
        "args": [
            847617
        ],
        "return": "even"
    },
    {
        "args": [
            348466
        ],
        "return": "even"
    }
]
```
## Credits

Found on Edabit: [Odds vs. Evens](https://edabit.com/challenge/uWpS5xMjzZFAkiQzL)
