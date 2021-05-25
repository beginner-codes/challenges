# Challenge 253 - Tile Teamwork Tactics

In a board game, a piece may advance 1-6 tiles forward depending on the number rolled on a six-sided dice. If you advance your piece onto the same tile as another player's piece, both of you earn a bonus.

Given you and your friend's tile number, create a function that returns if it's possible to earn a bonus when you roll the dice.

## Examples
```python
possible_bonus(3, 7) ➞ True

possible_bonus(1, 9) ➞ False

possible_bonus(5, 3) ➞ False
```
## Notes

- You cannot move backward (which is why example #3 doesn't work).
- If you are already on the same tile, return false, as you would be advancing away.
- Expect only positive integer inputs.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def possible_bonus(your_position: int, friends_position: int) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(possible_bonus(3, 7))

    def test_2(self):
        self.assertTrue(possible_bonus(0, 6))

    def test_3(self):
        self.assertTrue(possible_bonus(1, 6))

    def test_4(self):
        self.assertTrue(possible_bonus(2, 6))

    def test_5(self):
        self.assertTrue(possible_bonus(3, 6))

    def test_6(self):
        self.assertTrue(possible_bonus(4, 6))

    def test_7(self):
        self.assertTrue(possible_bonus(5, 6))

    def test_8(self):
        self.assertFalse(possible_bonus(6, 6))

    def test_9(self):
        self.assertFalse(possible_bonus(7, 6))

    def test_10(self):
        self.assertTrue(possible_bonus(23, 27))

    def test_11(self):
        self.assertFalse(possible_bonus(1, 9))

    def test_12(self):
        self.assertFalse(possible_bonus(5, 3))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Tile Teamwork Tactics](https://edabit.com/challenge/NHfYRHg2tDtcZyykB)
