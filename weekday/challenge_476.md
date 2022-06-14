# Challenge 476 - Chess Board Squares

Create a function that takes a chess board square's coordinate and return its color.

```
  a b cd ef g h
1 ⬛️⬜️⬛️⬜️⬛️⬜️⬛️⬜️
2 ⬜️⬛️⬜️⬛️⬜️⬛️⬜️⬛️
3 ⬛️⬜️⬛️⬜️⬛️⬜️⬛️⬜️
4 ⬜️⬛️⬜️⬛️⬜️⬛️⬜️⬛️
5 ⬛️⬜️⬛️⬜️⬛️⬜️⬛️⬜️
6 ⬜️⬛️⬜️⬛️⬜️⬛️⬜️⬛️
7 ⬛️⬜️⬛️⬜️⬛️⬜️⬛️⬜️
8 ⬜️⬛️⬜️⬛️⬜️⬛️⬜️⬛️
```
## Examples
```python
chess_board("a1") ➞ "black"

chess_board("e5") ➞ "black"

chess_board("d1") ➞ "white"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def chess_board(coordinate: str) -> str:
    return ""  # Put your code here!!!


test(476, chess_board)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "a1"
        ],
        "return": "black"
    },
    {
        "args": [
            "e5"
        ],
        "return": "black"
    },
    {
        "args": [
            "d1"
        ],
        "return": "white"
    },
    {
        "args": [
            "c7"
        ],
        "return": "black"
    },
    {
        "args": [
            "h5"
        ],
        "return": "white"
    },
    {
        "args": [
            "g2"
        ],
        "return": "white"
    },
    {
        "args": [
            "b3"
        ],
        "return": "white"
    },
    {
        "args": [
            "f6"
        ],
        "return": "black"
    },
    {
        "args": [
            "g5"
        ],
        "return": "black"
    }
]
```
## Credits

Found on Edabit: [Chess Board Squares](https://edabit.com/challenge/4BRGyox5xi8Kp7AAE)
