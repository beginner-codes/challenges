# Challenge 386 - Sum of Any Two Numbers Equal N

Create a function that takes a list of numbers and a number. Return `True` if the sum of any two elements is equal to that number. Otherwise, return `False`.

## Examples
```python
check_sum([10, 12, 4, 7, 9, 11], 16) ➞ True

check_sum([4, 5, 6, 7, 8, 9], 13) ➞ True

check_sum([0, 98, 76, 23], 174) ➞ True

check_sum([0, 9, 7, 23, 19, 18, 17, 66], 39) ➞ False

check_sum([2, 8, 9, 12, 45, 78], 1) ➞ False
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def check_sum(numbers: list[int], num: int) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(check_sum([10, 15, 3, 7], 17))

    def test_2(self):
        self.assertTrue(check_sum([4, 5, 6, 7, 8, 9], 13))

    def test_3(self):
        self.assertFalse(check_sum([2, 8, 9, 12, 45, 78], 1))

    def test_4(self):
        self.assertTrue(check_sum([10, 12, 4, 7, 9, 11], 16))

    def test_5(self):
        self.assertTrue(check_sum([0, 98, 76, 23], 174))

    def test_6(self):
        self.assertFalse(check_sum([0, 9, 7, 23, 19, 18, 17, 66], 39))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Sum of Two Numbers in List Equal to Given Number](https://edabit.com/challenge/KcnQtNoX5uC6PzpEF)
