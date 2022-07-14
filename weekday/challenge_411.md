# Challenge 411 - Poker Full House

Create a function that determines whether a player is holding a Full House in their hand. A hand is represented as a list of 5 cards. A full house is defined as a pair of cards and a three-of-a-kind.

To illustrate: `["A", "A", "A", "K", "K"]` would be a Full House, since the player holds 3 aces and a pair of kings.

## Examples
```python
is_full_house(["A", "A", "A", "K", "K"]) ➞ True

is_full_house(["3", "J", "J", "3", "3"]) ➞ True

is_full_house(["10", "J", "10", "10", "10"]) ➞ False

is_full_house(["7", "J", "3", "4", "2"]) ➞ False
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def is_full_house(hand: list[str]) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(is_full_house(["A", "A", "A", "K", "K"]))

    def test_2(self):
        self.assertTrue(is_full_house(["3", "J", "J", "3", "3"]))

    def test_3(self):
        self.assertTrue(is_full_house(["10", "J", "10", "J", "10"]))

    def test_4(self):
        self.assertFalse(is_full_house(["10", "J", "10", "10", "10"]))

    def test_5(self):
        self.assertFalse(is_full_house(["10", "J", "J", "2", "2"]))

    def test_6(self):
        self.assertFalse(is_full_house(["7", "J", "3", "4", "2"]))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Poker Full House](https://edabit.com/challenge/uugzpwJXKdiESZbjM)
