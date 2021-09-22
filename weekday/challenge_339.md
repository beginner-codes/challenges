# Challenge 339 - Consecutive Numbers

Create a function that determines whether elements in a list can be re-arranged to form a consecutive list of numbers where each number appears exactly once.

## Examples
```python
can_be_consecutive([5, 1, 4, 3, 2]) ➞ True
# Can be re-arranged to form [1, 2, 3, 4, 5]

can_be_consecutive([5, 1, 4, 3, 2, 8]) ➞ False

can_be_consecutive([5, 6, 7, 8, 9, 9]) ➞ False
# 9 appears twice
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def can_be_consecutive(numbers: list[int]) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(can_be_consecutive([5, 1, 4, 3, 2]))

    def test_2(self):
        self.assertTrue(can_be_consecutive([55, 59, 58, 56, 57]))

    def test_3(self):
        self.assertTrue(can_be_consecutive([-3, -2, -1, 1, 0]))

    def test_4(self):
        self.assertFalse(can_be_consecutive([5, 1, 4, 3, 2, 8]))

    def test_5(self):
        self.assertFalse(can_be_consecutive([5, 6, 7, 8, 9, 9]))

    def test_6(self):
        self.assertFalse(can_be_consecutive([5, 3]))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Consecutive Numbers](https://edabit.com/challenge/oKjqFFzaybbs8csiE)
