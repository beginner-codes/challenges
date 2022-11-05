# Challenge 567 - Read the Abacus

The Russian schoty is type of abacus (counting tool) that is used by sliding threaded beads along horizontal wires. An example schoty would have 7 wires, each holding 10 beads. Each bead, when moved to the left, would count as 1 unit. Starting from the bottom wire and moving up, the units increase by a factor of 10. If we use `"O"` for a bead and `"-"` to show the wire, we can represent the schoty as follows:
```
---OOOOOOOOOO  millions
---OOOOOOOOOO  hundred-thousands
---OOOOOOOOOO  ten-thousands
---OOOOOOOOOO  thousands
---OOOOOOOOOO  hundreds
---OOOOOOOOOO  tens
---OOOOOOOOOO  ones
```
To read the number, we count the beads on the left-hand side of each wire. In the example below, the number is `501264`:
```
---OOOOOOOOOO  0
OOOOO---OOOOO  5
---OOOOOOOOOO  0
O---OOOOOOOOO  1
OO---OOOOOOOO  2
OOOOOO---OOOO  6
OOOO---OOOOOO  4
```
Given a list of strings representing each wire in the schoty, return the number being displayed.

## Examples
```python
schoty([
  "---OOOOOOOOOO",
  "---OOOOOOOOOO",
  "---OOOOOOOOOO",
  "OOO---OOOOOOO",
  "O---OOOOOOOOO",
  "OOOOOOOOO---O",
  "OO---OOOOOOOO"
]) ➞ 3192

schoty([
  "OO---OOOOOOOO",
  "O---OOOOOOOOO",
  "OOOOO---OOOOO",
  "---OOOOOOOOOO",
  "---OOOOOOOOOO",
  "---OOOOOOOOOO",
  "---OOOOOOOOOO"
]) ➞ 2150000
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def schoty(beads: list[str]) -> int:
    return 0 # Put your code here!!!


test(567, schoty)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "OOOOOOOOO---O",
                "---OOOOOOOOOO",
                "OOOOO---OOOOO",
                "O---OOOOOOOOO",
                "OOOOOOOO---OO",
                "---OOOOOOOOOO",
                "OOOOOOOOO---O"
            ]
        ],
        "return": 9051809
    },
    {
        "args": [
            [
                "---OOOOOOOOOO",
                "OOOOOOOOO---O",
                "OOO---OOOOOOO",
                "---OOOOOOOOOO",
                "OO---OOOOOOOO",
                "OOOOOO---OOOO",
                "OOOOO---OOOOO"
            ]
        ],
        "return": 930265
    },
    {
        "args": [
            [
                "---OOOOOOOOOO",
                "---OOOOOOOOOO",
                "OOOO---OOOOOO",
                "OOOOOOO---OOO",
                "O---OOOOOOOOO",
                "OOOOOOOO---OO",
                "OOO---OOOOOOO"
            ]
        ],
        "return": 47183
    },
    {
        "args": [
            [
                "OO---OOOOOOOO",
                "OOOOOO---OOOO",
                "OOO---OOOOOOO",
                "OOO---OOOOOOO",
                "OOO---OOOOOOO",
                "OO---OOOOOOOO",
                "---OOOOOOOOOO"
            ]
        ],
        "return": 2633320
    },
    {
        "args": [
            [
                "OOOOO---OOOOO",
                "OOOOOOOO---OO",
                "OOOOOOOOO---O",
                "OOO---OOOOOOO",
                "O---OOOOOOOOO",
                "OOOOOOOOO---O",
                "OOOOOO---OOOO"
            ]
        ],
        "return": 5893196
    }
]
```
## Credits

Found on Edabit: [Read the Abacus (Part 1: Russian Schoty)](https://edabit.com/challenge/F64txHnfYj4e4MpAN)
