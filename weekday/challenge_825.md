# Challenge 825 - Roll the Dice

Write a function that returns the dice with the correct amount of eyes in a single string.

Dice:
```
 1    2    3    4    5    6
 
---  0--  0--  0-0  0-0  0-0
-0-  ---  -0-  ---  -0-  0-0
---  --0  --0  0-0  0-0  0-0
```
Your code would encode a 1 as a string in this format:
```
---/-O-/---
```
Write function that takes a number and returns the dice as a comma seperated string that add sum up to that number. Your function should find the fewest possible dice that sum to the value.

## Examples
```python
dice(3) ➞ "O--/-O-/--O"

dice(8) ➞ "O-O/O-O/O-O, O--/---/--O"

dice(6) ➞ "O-O/O-O/O-O"
```
## Notes

- The input is always a positive number
- Return an empty string when 0 is given

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


def dice(number: int) -> str:
    return ""  # Put your code here!!!


test(825, dice)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            3
        ],
        "return": "O--/-O-/--O"
    },
    {
        "args": [
            63
        ],
        "return": "O-O/O-O/O-O, O-O/O-O/O-O, O-O/O-O/O-O, O-O/O-O/O-O, O-O/O-O/O-O, O-O/O-O/O-O, O-O/O-O/O-O, O-O/O-O/O-O, O-O/O-O/O-O, O-O/O-O/O-O, O--/-O-/--O"
    },
    {
        "args": [
            11
        ],
        "return": "O-O/O-O/O-O, O-O/-O-/O-O"
    },
    {
        "args": [
            18
        ],
        "return": "O-O/O-O/O-O, O-O/O-O/O-O, O-O/O-O/O-O"
    },
    {
        "args": [
            6
        ],
        "return": "O-O/O-O/O-O"
    }
]
```

## Credits

Found on Edabit: [Roll the Dice](https://edabit.com/challenge/n5znbTz2vRcjqmnWt)
