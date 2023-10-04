# Challenge 764 - Hidden Calculator Words

At school, we used to play with our calculators and send each other secret messages. The trick was to enter a special number and turn the calculator upside-down. LOL ... I mean 707!

Given a number, create a function that converts it into a word by turning the integer 180 degrees around.
```
Number	Letter
1       I
2       Z
3       E
4       H
5       S
6       G
7       L
8       B
9       -
0       O
```

## Examples
```python
turn_calc(707) ➞ "LOL"

turn_calc(5508) ➞ "BOSS"

turn_calc(3045) ➞ "SHOE"
```

## Notes

- Convert to uppercase words.
- Ignore dots.

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


def turn_calc(number: int) -> str:
    return ""  # Put your code here!!!


test(764, turn_calc)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            5355378
        ],
        "return": "BLESSES"
    },
    {
        "args": [
            57108
        ],
        "return": "BOILS"
    },
    {
        "args": [
            0.7734
        ],
        "return": "HELLO"
    },
    {
        "args": [
            38076
        ],
        "return": "GLOBE"
    },
    {
        "args": [
            35380
        ],
        "return": "OBESE"
    }
]
```

## Credits

Found on Edabit: [Hidden Calculator Words](https://edabit.com/challenge/uRSeMB39t2g2jNpW9)
