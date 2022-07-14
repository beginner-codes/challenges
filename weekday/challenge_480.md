# Challenge 480 - Cup Swapping

There are three cups on a table, at positions `A`, `B`, and `C`. At the start, there is a ball hidden under the cup at position `B`.

However, I perform several swaps on the cups, which is notated as two letters. For example, if I swap the cups at positions `A` and `B`, I could notate this as `AB` or `BA`.

Create a function that returns the letter position that the ball is at, once I finish swapping the cups. The swaps will be given to you as a list.

## Worked Example
```python
cup_swapping(["AB", "CA", "AB"]) ➞ "C"

# Ball begins at position B.
# Cups A and B swap, so the ball is at position A.
# Cups C and A swap, so the ball is at position C.
# Cups A and B swap, but the ball is at position C, so it doesn't move.
```
## Examples
```python
cup_swapping(["AB", "CA"]) ➞ "C"

cup_swapping(["AC", "CA", "CA", "AC"]) ➞ "B"

cup_swapping(["BA", "AC", "CA", "BC"]) ➞ "A"
```
## Notes

- A swap could be notated in two different ways, since both ways end up with the same outcome.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def cup_swapping(swaps: list[str]) -> str:
    return ""  # Put your code here!!!


test(480, cup_swapping)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "AB",
                "CA"
            ]
        ],
        "return": "C"
    },
    {
        "args": [
            [
                "AB",
                "CA",
                "AB"
            ]
        ],
        "return": "C"
    },
    {
        "args": [
            [
                "AC",
                "CA",
                "CA",
                "AC"
            ]
        ],
        "return": "B"
    },
    {
        "args": [
            [
                "BA",
                "AC",
                "CA",
                "BC"
            ]
        ],
        "return": "A"
    },
    {
        "args": [
            [
                "BC",
                "CB",
                "CA",
                "BA"
            ]
        ],
        "return": "A"
    }
]
```
## Credits

Found on Edabit: [Cup Swapping](https://edabit.com/challenge/M47FDJLjfNoZ6k6gF)
