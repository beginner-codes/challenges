# Challenge 618 - Making Change

Create a function that takes an amount of monetary change (e.g. `47` cents) and breaks down the most efficient way that change can be made using USD quarters, dimes, nickels and pennies. Your function should return a dictionary.
```
Coin     Value
Penny    0.01
Nickel   0.05
Dime     0.10
Quarter  0.25
```
## Examples
```python
make_change(47) ➞ { "q": 1, "d": 2, "n": 0, "p": 2 }

make_change(24) ➞ { "q": 0, "d": 2, "n": 0, "p": 4 }

make_change(92) ➞ { "q": 3, "d": 1, "n": 1, "p": 2 }
```
## Notes

- Amount given will always be less than `100` and more than `0`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def make_change(amount: int) -> dict[str, int]:
    return {}  # Put your code here!!!


test(618, make_change)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            15
        ],
        "return": {
            "q": 0,
            "d": 1,
            "n": 1,
            "p": 0
        }
    },
    {
        "args": [
            92
        ],
        "return": {
            "q": 3,
            "d": 1,
            "n": 1,
            "p": 2
        }
    },
    {
        "args": [
            47
        ],
        "return": {
            "q": 1,
            "d": 2,
            "n": 0,
            "p": 2
        }
    },
    {
        "args": [
            24
        ],
        "return": {
            "q": 0,
            "d": 2,
            "n": 0,
            "p": 4
        }
    },
    {
        "args": [
            36
        ],
        "return": {
            "q": 1,
            "d": 1,
            "n": 0,
            "p": 1
        }
    }
]
```
## Credits

Found on Edabit: [Making Change](https://edabit.com/challenge/QDw3YayxCNqGaC9ji)
