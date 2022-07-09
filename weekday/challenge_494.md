# Challenge 494 - Poker Hand Ranking

In this challenge, you have to establish which kind of Poker combination is present in a deck of five cards. Every card is a string containing the card value (with the upper-case initial for face-cards) and the lower-case initial for suits, as in the examples below:

- `"Ah"` ➞ Ace of hearts
- `"Ks"` ➞ King of spades
- `"3d"` ➞ Three of diamonds
- `"Qc"` ➞ Queen of clubs
- 
There are 10 different combinations. Here's the list, in decreasing order of importance:
```
Name               Description
---------------------------------------------------------------------
Royal Flush        A, K, Q, J, 10, all with the same suit.
Straight Flush     Five cards in sequence, all with the same suit.
Four of a Kind     Four cards of the same rank.
Full House         Three of a Kind with a Pair.
Flush              Any five cards of the same suit, not in sequence.
Straight           Five cards in a sequence, but not of the same suit.
Three of a Kind    Three cards of the same rank.
Two Pair           Two different Pair.
Pair               Two cards of the same rank (2x K's, 2x 5's, etc..)
High Card          No other valid combination.
```
Given a list hand containing five strings being the cards, implement a function that returns a string with the name of the highest combination obtained, accordingly to the table above.

## Examples
```python
poker_hand_ranking(["10h", "Jh", "Qh", "Ah", "Kh"]) ➞ "Royal Flush"

poker_hand_ranking(["3h", "5h", "Qs", "9h", "Ad"]) ➞ "High Card"

poker_hand_ranking(["10s", "10c", "8d", "10d", "10h"]) ➞ "Four of a Kind"
```
## Notes

- For the purposes of this challenge, please consider Aces as high only.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def poker_hand_ranking(hand: list[str]) -> str:
    return ""  # Put your code here!!!


test(494, poker_hand_ranking)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "10h",
                "Jh",
                "Qh",
                "Ah",
                "Kh"
            ]
        ],
        "return": "Royal Flush"
    },
    {
        "args": [
            [
                "3h",
                "5h",
                "Qs",
                "9h",
                "Ad"
            ]
        ],
        "return": "High Card"
    },
    {
        "args": [
            [
                "10s",
                "10c",
                "8d",
                "10d",
                "10h"
            ]
        ],
        "return": "Four of a Kind"
    },
    {
        "args": [
            [
                "4h",
                "9s",
                "2s",
                "2d",
                "Ad"
            ]
        ],
        "return": "Pair"
    },
    {
        "args": [
            [
                "10s",
                "9s",
                "8s",
                "6s",
                "7s"
            ]
        ],
        "return": "Straight Flush"
    },
    {
        "args": [
            [
                "10c",
                "9c",
                "9s",
                "10s",
                "9h"
            ]
        ],
        "return": "Full House"
    },
    {
        "args": [
            [
                "8h",
                "2h",
                "8s",
                "3s",
                "3c"
            ]
        ],
        "return": "Two Pair"
    },
    {
        "args": [
            [
                "Jh",
                "9h",
                "7h",
                "5h",
                "2h"
            ]
        ],
        "return": "Flush"
    },
    {
        "args": [
            [
                "Ac",
                "Qc",
                "As",
                "Ah",
                "2d"
            ]
        ],
        "return": "Three of a Kind"
    },
    {
        "args": [
            [
                "Ad",
                "Kd",
                "Qd",
                "Jd",
                "9d"
            ]
        ],
        "return": "Flush"
    },
    {
        "args": [
            [
                "10h",
                "Jh",
                "Qs",
                "Ks",
                "Ac"
            ]
        ],
        "return": "Straight"
    },
    {
        "args": [
            [
                "3h",
                "8h",
                "2s",
                "3s",
                "3d"
            ]
        ],
        "return": "Three of a Kind"
    },
    {
        "args": [
            [
                "4h",
                "Ac",
                "4s",
                "4d",
                "4c"
            ]
        ],
        "return": "Four of a Kind"
    },
    {
        "args": [
            [
                "3h",
                "8h",
                "2s",
                "3s",
                "2d"
            ]
        ],
        "return": "Two Pair"
    },
    {
        "args": [
            [
                "8h",
                "8s",
                "As",
                "Qh",
                "Kh"
            ]
        ],
        "return": "Pair"
    },
    {
        "args": [
            [
                "Js",
                "Qs",
                "10s",
                "Ks",
                "As"
            ]
        ],
        "return": "Royal Flush"
    },
    {
        "args": [
            [
                "Ah",
                "3s",
                "4d",
                "Js",
                "Qd"
            ]
        ],
        "return": "High Card"
    }
]
```
## Credits

Found on Edabit: [Poker Hand Ranking](https://edabit.com/challenge/C6pHyc4iN6BNzmhsM)
