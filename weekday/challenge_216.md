# Challenge 216 - Don't Roll Doubles!

John is playing a dice game. The rules are as follows.

- Roll two dice.
- Add the numbers on the dice together.
- Add the total to your overall score.
- Repeat this for three rounds.
- But if you roll DOUBLES, your score is instantly wiped to 0 and your game ends immediately!

Create a function that takes in a list of tuples as input, and return John's score after his game has ended.

## Examples
```python
dice_game([(1, 2), (3, 4), (5, 6)]) ➞ 21

dice_game([(1, 1), (5, 6), (6, 4)]) ➞ 0

dice_game([(4, 5), (4, 5), (4, 5)]) ➞ 27
```
## Notes

- Ignore all other tuples in the list if a throw happens to be doubles and go straight to returning `0`.
- John only has two dice and will always give you outcomes for three rounds.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


Roll = tuple[int, int]


def dice_game(rolls: list[Roll]) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(dice_game([(1, 2), (3, 4), (5, 6)]), 21)

    def test_2(self):
        self.assertEqual(dice_game([(1, 1), (5, 6), (6, 4)]), 0)

    def test_3(self):
        self.assertEqual(dice_game([(4, 5), (4, 5), (4, 5)]), 27)

    def test_4(self):
        self.assertEqual(dice_game([(1, 3), (4, 3), (5, 2)]), 18)

    def test_5(self):
        self.assertEqual(dice_game([(1, 3), (4, 3), (5, 5)]), 0)

    def test_6(self):
        self.assertEqual(dice_game([(1, 3), (4, 4), (5, 2)]), 0)

    def test_7(self):
        self.assertEqual(dice_game([(5, 6), (5, 6), (5, 6)]), 33)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Don't Roll Doubles!](https://edabit.com/challenge/qeyinsjZHCPEddbfe)
