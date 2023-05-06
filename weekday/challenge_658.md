# Challenge 658 - Heroes vs. Monsters: a Role Playing Game Battle System

You are implementing a battle system for a simple role-playing game. A hero is fighting various monsters, and you have to determine the battle's outcome for each engaged skirmish. Hero and monsters share some stats:

- `HP` or Health Points: The amount of damage the character can sustain. If it reaches 0 (or less) the character dies.
- `ATT` or Attack: The character offensive capacity.
- `DEF` or Defense: The character defensive capacity.

For either hero and monster, the damage inflicted is calculated subtracting the opponent's defense score from the attacker doubled attack score.

In each round hero attacks first, and his damage rate is subtracted from the monster's `HP`. If the monster survives (`HP > 0`), it is his turn to attack. If the hero survives (`HP > 0`), a new round starts. The hero can also have some `POT`, or Healing Potions, in his backpack: only when his `HP` is equal to or lower than `10`, a potion can (and must) be used for regaining `10 HP` at the start of a new round. When the hero heals, he can't attack, but he receives only half damage from the monster's attack. Every potion can be used only once, then it must be discarded.

Given a dictionary containing the character's stats (with p-prefix ones being the hero's stats and m-prefix ones being the monster's) you must return a string:

- `"Victory in x rounds"` if the hero wins.
- `"Game Over in x rounds"` if the monster wins.

`x` being the number of rounds elapsed.

## Examples
```python
battle({
  "pHP": 12,
  "pATT": 10,
  "pDEF": 10,
  "pPOT": 0,
  "mHP": 20,
  "mATT": 6,
  "mDEF": 14
}) ➞ "Victory in 4 rounds"

# Hero's damage rate = (10 * 2) - 14 = 6
# Monster's damage rate = (6 * 2) - 10 = 2
# Round 1: mHP - 6 = 14, pHP - 2 = 10
# Round 2: No potions to use! mHP - 6 = 8, pHP - 2 = 8
# Round 3: mHP - 6 = 2, pHP - 2 = 6
# Round 4: mHP - 6 = -4 ... monster is dead

battle({
  "pHP": 10,
  "pATT": 10,
  "pDEF": 10,
  "pPOT": 2,
  "mHP": 10,
  "mATT": 8,
  "mDEF": 14
}) ➞ "Victory in 3 rounds"

# Hero's damage = 6, monster's damage = 6
# Round 1: mHp - 6 = 4, pHP - 6 = 4
# Round 2: Player uses a potion, heals 10 HP, receive half the monster damage, pHP = 11
# Round 3: mHP - 6 = -2 ... monster is dead

battle({
  "pHP": 12,
  "pATT": 7,
  "pDEF": 6,
  "pPOT": 2,
  "mHP": 30,
  "mATT": 8,
  "mDEF": 10
}) ➞ "Game Over in 5 rounds"

# Hero's damage rate = 4, Monster's damage rate = 10
# Round 1: mHP - 4 = 26, pHP - 10 = 2
# Round 2: Hero heals 10 hp, monster hit for 5 HP, pHP = 7
# Round 3: Hero heals 10 hp, monster hit for 5 HP, pHP = 12
# Round 4: mHP - 4 = 22, pHP - 10 = 2
# Round 5: No potions to use! mHP - 4 = 18, pHP - 10 = -8 ... hero is dead
```
## Notes

- Hero attacks (or heals) first in each round.
- A potion must be used when HP is equal to or less than 10, except on the first round.
- When the hero uses a potion, he can't attack the monster in the same round, but he can defend from the monster's attack, receiving only half the damage.
- Remember to discard the potion after using it.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def battle(stats: dict[str, int]) -> str:
    return ""  # Put your code here!!!


test(658, battle)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            {
                "pHP": 10,
                "pATT": 10,
                "pDEF": 10,
                "pPOT": 0,
                "mHP": 20,
                "mATT": 6,
                "mDEF": 14
            }
        ],
        "return": "Victory in 4 rounds"
    },
    {
        "args": [
            {
                "pHP": 100,
                "pATT": 12,
                "pDEF": 8,
                "pPOT": 3,
                "mHP": 200,
                "mATT": 14,
                "mDEF": 8
            }
        ],
        "return": "Game Over in 5 rounds"
    },
    {
        "args": [
            {
                "pHP": 10,
                "pATT": 10,
                "pDEF": 10,
                "pPOT": 2,
                "mHP": 10,
                "mATT": 8,
                "mDEF": 14
            }
        ],
        "return": "Victory in 3 rounds"
    },
    {
        "args": [
            {
                "pHP": 1480,
                "pATT": 16,
                "pDEF": 16,
                "pPOT": 4,
                "mHP": 860,
                "mATT": 14,
                "mDEF": 20
            }
        ],
        "return": "Victory in 72 rounds"
    },
    {
        "args": [
            {
                "pHP": 300,
                "pATT": 5,
                "pDEF": 4,
                "pPOT": 0,
                "mHP": 120,
                "mATT": 10,
                "mDEF": 6
            }
        ],
        "return": "Game Over in 19 rounds"
    }
]
```
## Credits

Found on Edabit: [Heroes vs. Monsters: a Role Playing Game Battle System](https://edabit.com/challenge/y3CEwBrJqqkeefgnt)
