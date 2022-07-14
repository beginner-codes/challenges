# Challenge 430 - Gold Distribution

A group of pirates each have a distribution of gold coins, which can be represented as a list:
```python
[3, 9, 4, 5, 5]
# Pirate 1 has 3 gold, Pirate 2 has 9 gold, etc.
The difference between each pirate's share of gold and that of the richest pirate is represented as:

[6, 0, 5, 4, 4]
# Since 6 = 9 - 3, 0 = 9 - 9, 4 = 9 - 5, etc.
```
Pirates have a keen sense of fairness, and a pirate will kill the others if he deems his share to be too little. Each pirate has a unique inequality threshold - the maximum difference he is willing to tolerate before he kills his comrades.

Using the above gold distribution:
```python
[5, 0, 5, 5, 5]
# Pirates killed, since 5 < 6.
# 5 is Pirate 1's inequality distribution and 6 is his gold difference.

[7, 0, 5, 5, 5]
# Pirate 1 is satisfied, since 7 > 6.
# All other pirates are satisfied as well.
```
Given a distribution of coins and a list of inequality thresholds, create a function that returns `True` if any pirates are killed, or `False` otherwise.

## Examples
```python
pirates_killed([3, 5, 8, 3, 4], [10, 4, 2, 5, 5]) ➞ False

pirates_killed([3, 5, 8, 3, 4], [10, 4, 2, 5, 1]) ➞ True

pirates_killed([3, 3, 10], [7, 7, 0]) ➞ False

pirates_killed([3, 3, 10], [6, 6, 0]) ➞ True
```
## Notes

- A pirate kills if the difference in his share of gold from the richest pirate is strictly greater than his inequality threshold.
- Gold and inequality distribution lists are both ordered the same. (e.g. Pirate 1 is index 0 for both lists, Pirate 2 is index 1 for both lists, etc.).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def pirates_killed(gold: list[int], thresholds: list[int]) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertFalse(pirates_killed([3, 5, 8, 3, 4], [10, 4, 2, 5, 5]))

    def test_2(self):
        self.assertTrue(pirates_killed([3, 5, 8, 3, 4], [10, 4, 2, 5, 1]))

    def test_3(self):
        self.assertFalse(pirates_killed([3, 3, 10], [7, 7, 0]))

    def test_4(self):
        self.assertTrue(pirates_killed([3, 3, 10], [6, 6, 0]))

    def test_5(self):
        self.assertFalse(pirates_killed([3, 3, 3], [0, 0, 0]))

    def test_6(self):
        self.assertTrue(pirates_killed([3, 3, 4, 4], [0, 0, 1, 1]))

    def test_7(self):
        self.assertFalse(pirates_killed([3, 3, 4, 4], [1, 1, 0, 0]))

    def test_8(self):
        self.assertTrue(pirates_killed([3, 3, 4, 4], [0, 0, 0, 1]))

    def test_9(self):
        self.assertTrue(pirates_killed([3, 3, 4, 4, 5], [0, 0, 0, 1, 1]))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Gold Distribution](https://edabit.com/challenge/eraBhwF8HkJDAa2pS)
