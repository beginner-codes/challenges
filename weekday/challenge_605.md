# Challenge 605 - Coin Co-Operation

Let's say that there exists a machine that gives out free coins, but with a twist!

Separating two people is a wall, and this machine is placed in such a way that both people are able to access it. Spending a coin in this machine will give the person on the other side 3 coins and vice versa.

If both people continually spend coins for each other (SHARING), then they'll both gain a net profit of 2 coins per turn. However, there is always the possibility for someone to act selfishly (STEALING): they spend no coins, yet they still receive the generous 3 coin gift from the other person!

*The Challenge*

Assuming that both people start with 3 coins each, create a function that calculates both people's final number of coins. You will be given two lists of strings, with each string being the words `'share'` or `'steal'`.

## Examples
```python
get_coin_balances(["share"], ["share"]) ➞ [5, 5]
# Both people spend one coin, and receive 3 coins each.

get_coin_balances(["steal"], ["share"]) ➞ [6, 2]
# Person 1 gains 3 coins, while person 2 loses a coin.

get_coin_balances(["steal"], ["steal"]) ➞ [3, 3]
# Neither person spends any coins and so no one gets rewarded.

get_coin_balances(["share", "share", "share"], ["steal", "share", "steal"]) ➞ [3, 11]
```
## Notes

- No tests will include a negative number of coins.
- All words will be given in lowercase.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def get_coin_balances(person_a: list[str], person_b: list[str]) -> list[int]:
    return []  # Put your code here!!!


test(605, get_coin_balances)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "share"
            ],
            [
                "steal"
            ]
        ],
        "return": [
            2,
            6
        ]
    },
    {
        "args": [
            [
                "steal"
            ],
            [
                "share"
            ]
        ],
        "return": [
            6,
            2
        ]
    },
    {
        "args": [
            [
                "steal",
                "steal"
            ],
            [
                "share",
                "share"
            ]
        ],
        "return": [
            9,
            1
        ]
    },
    {
        "args": [
            [
                "share",
                "share",
                "share"
            ],
            [
                "steal",
                "share",
                "steal"
            ]
        ],
        "return": [
            3,
            11
        ]
    },
    {
        "args": [
            [
                "steal",
                "steal",
                "steal",
                "steal"
            ],
            [
                "steal",
                "steal",
                "steal",
                "steal"
            ]
        ],
        "return": [
            3,
            3
        ]
    }
]
```
## Credits

Found on Edabit: [Coin Co-Operation](https://edabit.com/challenge/8NyNftbNXd6CZCDXf)
