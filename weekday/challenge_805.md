# Challenge 805 - Pokemon Damage Calculator

It's a Pokemon battle! Your task is to calculate the damage that a particular move would do using the following formula (not the actual one from the game):
```
damage = 50 * (attack / defense) * effectiveness
```
- attack = your attack power
- defense = the opponent's defense
- effectiveness = the effectiveness of the attack based on the matchup (see explanation below)

**Effectiveness:**

Attacks can be super effective, neutral, or not very effective depending on the match-up. For example, water would be super effective against fire, but not very effective against grass.

- Super effective: 2x damage
- Neutral: 1x damage
- Not very effective: 0.5x damage

To prevent this challenge from being tedious, you'll only be dealing with four types: fire, water, grass, and electric. Here is the effectiveness of each match-up:
```
fire > grass
fire < water
fire = electric
water < grass
water < electric
grass = electric
```
The function you must implement takes in:

- your type
- the opponent's type
- your attack power
- the opponent's defense

## Examples
```python
calculate_damage("fire", "water", 100, 100) ➞ 25

calculate_damage("grass", "fire", 35, 5) ➞ 175

calculate_damage("electric", "fire", 100, 100) ➞ 50
```
## Notes

- Any type against itself is not very effective
- Assume that the relationships between different types are symmetric (if A is super effective against B, then B is not very effective against A).

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
from typing import Literal, Union
from beginnercodes.challenges import test


Types = Union[Literal["electric"], Literal["fire"], Literal["grass"], Literal["water"]]


def calculate_damage(my_type: Types, their_type: Types, my_attack: int, their_defence: int) -> int:
    return 0  # Put your code here!!!


test(805, calculate_damage)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            "fire",
            "water",
            100,
            100
        ],
        "return": 25
    },
    {
        "args": [
            "grass",
            "fire",
            35,
            5
        ],
        "return": 175
    },
    {
        "args": [
            "grass",
            "electric",
            57,
            19
        ],
        "return": 150
    },
    {
        "args": [
            "fire",
            "electric",
            10,
            2
        ],
        "return": 250
    },
    {
        "args": [
            "grass",
            "water",
            100,
            100
        ],
        "return": 100
    }
]
```

## Credits

Found on Edabit: [Pokemon Damage Calculator](https://edabit.com/challenge/pzQXHMqizBmaLDCHc)
