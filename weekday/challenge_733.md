# Challenge 733 - East or West

You will be given a list of string `"east"` formatted differently every time. Create a function that returns `"west"`
wherever there is `"east"`. Format the string according to the input. Check the examples below to better understand the
question.

## Examples

```python
direction(["east", "EAST", "eastEAST"]) ➞ ["west", "WEST", "westWEST"]

direction(["eAsT EaSt", "EaSt eAsT"]) ➞ ["wEsT WeSt", "WeSt wEsT"]

direction(["east EAST", "e a s t", "E A S T"]) ➞ ["west WEST", "w e s t", "W E S T"]
```

## Notes

- The input will only be `"east"` in different formats.

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


def direction(east: list[str]) -> list[str]:
    return []  # Put your code here!!!


test(733, direction)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
  {
    "args": [
      [
        "east",
        "EAST",
        "eastEAST"
      ]
    ],
    "return": [
      "west",
      "WEST",
      "westWEST"
    ]
  },
  {
    "args": [
      [
        "eAsT EaSt",
        "EaSt eAsT"
      ]
    ],
    "return": [
      "wEsT WeSt",
      "WeSt wEsT"
    ]
  },
  {
    "args": [
      [
        "east EAST",
        "e a s t",
        "E A S T"
      ]
    ],
    "return": [
      "west WEST",
      "w e s t",
      "W E S T"
    ]
  }
]
```

## Credits

Found on Edabit: [East or West](https://edabit.com/challenge/39utPCHvtWqt5vaz9)
