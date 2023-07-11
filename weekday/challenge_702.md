# Challenge 702 - Dance for Cash!

Your local bank has decided to upgrade its ATMs by incorporating motion sensor technology. The machines now interpret uses a series of dance moves in place of a PIN.

Create a function that converts a customer's PIN to its dance equivalent. There is one dance move per digit in the PIN:

- 0 => Shimmy
- 1 => Shake
- 2 => Pirouette
- 3 => Slide
- 4 => Box Step
- 5 => Headspin
- 6 => Dosado
- 7 => Pop
- 8 => Lock
- 9 => Arabesque

## Examples
```python
dance_convert("0000") ➞ ["Shimmy", "Shake", "Pirouette", "Slide"]

dance_convert("3856") ➞ [ "Slide", "Arabesque", "Pop", "Arabesque" ]

dance_convert("9999") ➞ [ "Arabesque", "Shimmy", "Shake", "Pirouette" ]

dance_convert("32a1") ➞ "Invalid input."
```
## Notes

- Valid input will always be a string of four digits. Output will be a list of strings.
- If the input is not four valid integers, return the string, `"Invalid input."`

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def widen_streets(buildings: list[str], width: int) -> list[str]:
    return []  # Put your code here!!!


test(701, widen_streets)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "3619"
        ],
        "return": [
            "Slide",
            "Pop",
            "Slide",
            "Pirouette"
        ]
    },
    {
        "args": [
            "9104"
        ],
        "return": [
            "Arabesque",
            "Pirouette",
            "Pirouette",
            "Pop"
        ]
    },
    {
        "args": [
            "0123"
        ],
        "return": [
            "Shimmy",
            "Pirouette",
            "Box Step",
            "Dosado"
        ]
    },
    {
        "args": [
            "8765"
        ],
        "return": [
            "Lock",
            "Lock",
            "Lock",
            "Lock"
        ]
    },
    {
        "args": [
            "834"
        ],
        "return": "Invalid input."
    }
]
```
## Credits

Found on Edabit: [Dance for Cash!](https://edabit.com/challenge/kSHpZ3KguSDSb5cwx)
