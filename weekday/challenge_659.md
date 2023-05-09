# Challenge 659 - Lottery Ticket

Given a lottery ticket represented by a list of 2-value lists, create a function to find out if you've won the jackpot.

To do this, you must first count the "mini-wins" on your ticket. Each sublist has both a string and a number within it. If the character code of any characters in the string matches the number, you get a mini-win. Note you can only have one mini-win per sublist.

Once you have counted all of your mini-wins, compare that number to the `win` value. If your number of mini-wins is more than or equal to `win`, return `Winner!`. Else, return `Loser!`.

## Examples
```python
lottery([["YYW", 70], ["WXK", 65], ["RPDI", 88]], 2)
➞ "Loser!"

lottery([["KG", 80], ["NTBBVZ", 79], ["CI", 73], ["AGXMEE", 74], ["IU", 68], ["VOSP" , 84]], 1)
➞ "Winner!"

lottery([["ZSAMZB", 81], ["XWWCXP", 72], ["SYBRQOHP", 88], ["HJSVV", 75]], 1)
➞ "Loser!"
```
## Notes

- All inputs will be in the correct format.
- Strings on ticket are not always the same length.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def lottery(ticket: list[list[str | int]], win: int) -> str:
    return ""  # Put your code here!!!


test(659, lottery)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                [
                    "XONLHEB",
                    71
                ],
                [
                    "FXMR",
                    65
                ],
                [
                    "WMGY",
                    89
                ]
            ],
            1
        ],
        "return": "Winner!"
    },
    {
        "args": [
            [
                [
                    "KG",
                    80
                ],
                [
                    "NTBBVZ",
                    79
                ],
                [
                    "CI",
                    73
                ],
                [
                    "AGXMEE",
                    74
                ],
                [
                    "IU",
                    68
                ],
                [
                    "VOSP",
                    84
                ]
            ],
            1
        ],
        "return": "Winner!"
    },
    {
        "args": [
            [
                [
                    "TRJZKKCQ",
                    81
                ],
                [
                    "KYC",
                    80
                ],
                [
                    "WU",
                    66
                ],
                [
                    "MFTWCFZ",
                    83
                ],
                [
                    "TNIRSP",
                    72
                ],
                [
                    "VC",
                    86
                ],
                [
                    "AINOS",
                    87
                ],
                [
                    "RGROXMF",
                    86
                ],
                [
                    "URKVFY",
                    70
                ]
            ],
            3
        ],
        "return": "Winner!"
    },
    {
        "args": [
            [
                [
                    "YYW",
                    70
                ],
                [
                    "WXK",
                    65
                ],
                [
                    "RPDI",
                    88
                ]
            ],
            2
        ],
        "return": "Loser!"
    },
    {
        "args": [
            [
                [
                    "SHUT",
                    85
                ],
                [
                    "DOWPKSLD",
                    80
                ],
                [
                    "QOOGBTDG",
                    85
                ],
                [
                    "EID",
                    68
                ],
                [
                    "EZKKAEYW",
                    81
                ],
                [
                    "OYQBJCJE",
                    86
                ],
                [
                    "WYTDAMFI",
                    87
                ],
                [
                    "CW",
                    89
                ],
                [
                    "BICKVN",
                    76
                ],
                [
                    "BQH",
                    79
                ]
            ],
            3
        ],
        "return": "Winner!"
    }
]
```
## Credits

Found on Edabit: [Lottery Ticket](https://edabit.com/challenge/EJ2RqF9AEmk64mLsv)
