# Challenge 780 - Add Dollar Bills

Create a function that takes a string containing money in dollars and pounds sterling (seperated by comma) and returns the sum of dollars only, as an integer.

For the input string:

- Each amount is prefixed by the currency symbol: `d` for dollars and `p` for pounds.
- Thousands are represented by the suffix k. (i.e. d4k = $4,000 and p40k = £40,000)

## Examples
```python
add_bill("d20,p40,p60,d50") ➞ 20 + 50 = 70

add_bill("p30,d20,p60,d150,p360") ➞ 20  + 150 = 170

add_bill("p30,d2k,p60,d200,p360") ➞ 2 * 1000 + 200 = 2200
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. *
*[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a
key `args` that are a list of parameters your function should take. The `return` key is what your function should return
given the `args`.

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your
solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:

```python
from __future__ import annotations
from beginnercodes.challenges import test


def add_bill(money: str) -> int:
    return 0  # Put your code here!!!


test(780, add_bill)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            "d10k,p500,p200"
        ],
        "return": 10000
    },
    {
        "args": [
            "d20k,d100,p40"
        ],
        "return": 20100
    },
    {
        "args": [
            "d10,d40,p60,d200"
        ],
        "return": 250
    },
    {
        "args": [
            "d200,p40,p60,d1k"
        ],
        "return": 1200
    },
    {
        "args": [
            "p20k,p100,d100"
        ],
        "return": 100
    }
]
```

## Credits

Found on Edabit: [Add Dollar Bills](https://edabit.com/challenge/rBMsnM8HuGNSwkBCR)
