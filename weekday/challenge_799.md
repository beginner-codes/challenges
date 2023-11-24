# Challenge 799 - House of Cards

The diagram below shows a sequence of larger and larger houses of cards, with the total number of cards included for each:
```
/ \      /_\          /_\             /_\
       / \ / \      /_\ /_\         /_\ /_\
                  / \ / \ / \     /_\ /_\ /_\
                                / \ / \ / \ / \
 2        7           15              26
```

Given the tower height, return the number of cards needed to construct a full house of cards.

## Examples
```python
cards_needed(3) ➞ 15

cards_needed(4) ➞ 26

cards_needed(0) ➞ 0
```
## Notes

- The height should always be equal or greater than 0. Return `"invalid"` if the value given doesn't abide by this rule.

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


def cards_needed(height: int) -> int:
    return 0  # Put your code here!!!


test(799, cards_needed)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            36
        ],
        "return": 1962
    },
    {
        "args": [
            7
        ],
        "return": 77
    },
    {
        "args": [
            29
        ],
        "return": 1276
    },
    {
        "args": [
            38
        ],
        "return": 2185
    },
    {
        "args": [
            -1
        ],
        "return": "invalid"
    }
]
```

## Credits

Found on Edabit: [House of Cards](https://edabit.com/challenge/kPDSPe9cHwbE2jANs)
