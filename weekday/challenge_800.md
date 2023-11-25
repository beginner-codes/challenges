# Challenge 800 - The Primiera

Primiera (from the French word prime, "prize") is a combination of cards of Scopa, a popular Italian card game.

For establishing the value of the Primiera, a separate point scale is used for selecting the best cards in the player's deck, in each of the four suits and totaling those four cards point values. A Primiera requires at least one card for each suit, otherwise, it can't be calculated.

This is the Primiera points scale:

- 7 is worth 21 points.
- 6 is worth 18 points.
- Ace is worth 16 points.
- Cards from 2 to 5 are worth 10 points plus the card value.
- Face cards (Jack, Queen and King) are worth 10 points.
- Create a function that takes in a list representing a cards deck and returns the value of the Primiera.

## Examples
```python
get_primiera_score(["Ad", "7d", "5h", "2c", "Ks"]) ➞ 58
# In the diamonds set 7 is higher than Ace (21 > 16).

get_primiera_score(["2d", "Jd", "7h", "Qc", "5s", "As"]) ➞ 59
# In the diamonds set 2 is higher than Jack (12 > 10), while in
# the spades set Ace is higher than 5 (16 > 15 ).

get_primiera_score(["2d", "Jd", "Qc", "5s", "As"]) ➞ 0
# There aren't cards in the hearts set, so Primiera can't be
# calculated.
```
## Notes

- Notation: A=Ace, card numbers from 2 to 7, J=Jack, Q=Queen, or K=King + d=diamonds, h=hearts, c=clubs, or s=spades.
- If one or more suits are missing from the deck the value of the Primiera is equal to 0.

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


def get_primiera_score(cards: list[str]) -> int:
    return 0  # Put your code here!!!


test(800, get_primiera_score)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                "7d",
                "Ad",
                "Kd",
                "2h",
                "6h",
                "5h",
                "Ah",
                "3c",
                "Jc",
                "Ac",
                "7c",
                "3c",
                "4c"
            ]
        ],
        "return": 0
    },
    {
        "args": [
            [
                "5d",
                "7h",
                "Qc",
                "Ac",
                "4c",
                "Kc",
                "As"
            ]
        ],
        "return": 68
    },
    {
        "args": [
            [
                "3d",
                "7d",
                "Kd",
                "7h",
                "Qh",
                "Ah",
                "7s",
                "3c",
                "Jc"
            ]
        ],
        "return": 76
    },
    {
        "args": [
            [
                "3d",
                "6d",
                "6h",
                "Qh",
                "7s",
                "As",
                "6c",
                "Jc"
            ]
        ],
        "return": 75
    }
]
```

## Credits

Found on Edabit: [The Primiera](https://edabit.com/challenge/bPzBa5JKvb6XFyKMs)
