# Challenge 572 - No Good Numbers

A positive number's population is the sum of 1's in its binary representation.

- An `"evil"` number has an even numbered population.
- An `"odious"` number has an odd numbered population.
- A number is `"pernicious"` if its population is a prime number.

Create a function that takes a number as an argument and returns a sorted list of all its descriptors (`"Evil"`, `"Odious"`, or `"Pernicious"`).

## Examples
```python
how_bad(7) ➞ ["Odious", "Pernicious"]
# 7 in binary is "111".
# 1 + 1 + 1 = 3 in "111" means "Odious" should be added to the list answer.
# 3 is a prime number, meaning "Pernicious" should also be added.

how_bad(17) ➞ ["Evil", "Pernicious"]
# 17 in binary is "10001".
# 1 + 1 = 2 in "10001" means "Evil" should be added to the list answer.
# 2 is a prime number, meaning "Pernicious" should also be added.

how_bad(23) ➞ ["Evil"]
# 23 in binary is "10111".
# Four 1's in "10111" means "Evil" should be added to the list answer.
# 4 is not a prime number, meaning "Pernicious" should not be added.
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def how_bad(number: int) -> list[str]:
    return []  # Put your code here!!!


test(572, how_bad)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            98765
        ],
        "return": [
            "Evil"
        ]
    },
    {
        "args": [
            97
        ],
        "return": [
            "Odious",
            "Pernicious"
        ]
    },
    {
        "args": [
            7
        ],
        "return": [
            "Odious",
            "Pernicious"
        ]
    },
    {
        "args": [
            66
        ],
        "return": [
            "Evil",
            "Pernicious"
        ]
    },
    {
        "args": [
            77
        ],
        "return": [
            "Evil"
        ]
    }
]
```
## Credits

Found on Edabit: [No Good Numbers](https://edabit.com/challenge/WixXhsdqcNHe3vTn3)
