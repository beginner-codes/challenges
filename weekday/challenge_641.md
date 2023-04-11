# Challenge 641 - Blackjack

Create a function that takes a list of card numbers and checks if the sum of their value exceeds 21. If the sum exceeds 21, return `True` and if the sum is under or equal to 21, return `False`. Values of the cards are as follows:

- 2-10 are their value.
- J-K (face cards) count as 10.
- Aces count either as 1 or 11 - play conservatively, so that if giving an ace a value of 11 causes you to lose and 1 allows you to win, then go with 1.

## Examples
```python
over_twenty_one([2, 8, "J"]) ➞ False

over_twenty_one(["A", "J", "K"]) ➞ False

over_twenty_one([5, 5, 3, 9]) ➞ True

over_twenty_one([2, 6, 4, 4, 5]) ➞ False

over_twenty_one(["J", "Q", "K"]) ➞ True
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def over_twenty_one(cardes: list[int | str]) -> bool:
    return False  # Put your code here!!!


test(641, over_twenty_one)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                5,
                3,
                6,
                6,
                7,
                9
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                "A",
                2,
                3
            ]
        ],
        "return": false
    },
    {
        "args": [
            [
                "A",
                "J",
                "K",
                "Q"
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                "A",
                "J",
                "K"
            ]
        ],
        "return": false
    }
]
```
## Credits

Found on Edabit: [Blackjack](https://edabit.com/challenge/d4YpsSWkDvgefxBc4)
