# Challenge 223 - Are the Sum of Digits in the Numbers Equal?

Write a function that takes a list of numbers and determines if the sum of the digits in each number are equal to each other.

## Examples
```python
is_equal([105, 42]) ➞ True
# 1 + 0 + 5 = 6
# 4 + 2 = 6

is_equal([21, 35]) ➞ False

is_equal([0, 0]) ➞ True
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def is_equal(numbers: list[int]) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(is_equal([11, 20]))

    def test_2(self):
        self.assertFalse(is_equal([14, 21]))

    def test_3(self):
        self.assertTrue(is_equal([0, 0]))

    def test_4(self):
        self.assertFalse(is_equal([101, 201]))

    def test_5(self):
        self.assertTrue(is_equal([102, 201, 300]))

    def test_6(self):
        self.assertFalse(is_equal([101, 201, 301]))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Are the Sum of Digits in the Numbers Equal?](https://edabit.com/challenge/zgu7m6W7i3z5SYwa6)
