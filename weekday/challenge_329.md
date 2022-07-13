# Challenge 329 - Numbered Cards

You have a pack of 5 randomly numbered cards, which can range from `0`-`9`. You can win if you can produce a higher two-digit number from your cards, than your opponent. Write a function that returns `True` if your cards win that round.

## Worked Example
```python
win_round([2, 5, 2, 6, 9], [3, 7, 3, 1, 2]) ➞ True
# Your cards can make the number 96
# Your opponent can make the number 73
# You win the round since 96 > 73
```
## Examples
```python
win_round([2, 5, 2, 6, 9], [3, 7, 3, 1, 2]) ➞ True

win_round([1, 2, 3, 4, 5], [9, 8, 7, 6, 5]) ➞ False

win_round([4, 3, 4, 4, 5], [3, 2, 5, 4, 1]) ➞ False
```
## Notes

- Return `False` if you and your opponent reach the same maximum number

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def win_round(players_hand: list[int], opponents_hand: list[int]) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(win_round([2, 5, 2, 6, 9], [3, 7, 3, 1, 2]))

    def test_2(self):
        self.assertFalse(win_round([1, 2, 3, 4, 5], [9, 8, 7, 6, 5]))

    def test_3(self):
        self.assertFalse(win_round([4, 3, 4, 4, 5], [3, 2, 5, 4, 1]))

    def test_4(self):
        self.assertTrue(win_round([3, 2, 8, 9, 4], [0, 7, 9, 3, 1]))

    def test_5(self):
        self.assertTrue(win_round([1, 4, 9, 2, 1], [3, 7, 7, 8, 7]))

    def test_6(self):
        self.assertTrue(win_round([6, 5, 5, 8, 5], [6, 2, 5, 2, 5]))

    def test_7(self):
        self.assertFalse(win_round([5, 3, 5, 9, 2], [5, 9, 2, 8, 0]))

    def test_8(self):
        self.assertFalse(win_round([3, 2, 0, 3, 5], [7, 5, 8, 6, 2]))

    def test_9(self):
        self.assertTrue(win_round([4, 1, 0, 2, 9], [3, 5, 5, 2, 8]))

    def test_10(self):
        self.assertTrue(win_round([9, 8, 7, 3, 4], [5, 3, 4, 7, 9]))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Numbered Cards](https://edabit.com/challenge/rnvBtoNMBtznXLhs8)
