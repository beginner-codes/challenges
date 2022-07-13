# Challenge 374 - Basic Statistics: Median

The median of a group of numbers is the middle number when the group is sorted. If the size of the group is even, the median is the average of the middle two numbers. Given a sorted list of numbers, return the median (rounded to one decimal place if the median isn't an integer).

## Examples
```python
median([1, 2, 4, 5, 6, 8, 8, 8, 10]) ➞ 6

median([2, 2, 6, 8, 8, 10, 10]) ➞ 8

median([1, 2, 2, 4, 7, 8, 9, 10]) ➞ 5.5
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def median(numbers: list[int]) -> float:
    return 0.0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(median([3, 4, 4, 5, 6, 8]), 4.5)

    def test_2(self):
        self.assertEqual(median([1, 4, 4, 9, 9, 10]), 6.5)

    def test_3(self):
        self.assertEqual(median([1, 2, 4, 4, 4, 7, 7, 9, 10]), 4)

    def test_4(self):
        self.assertEqual(median([1, 7, 8, 8, 10, 10, 10]), 8)

    def test_5(self):
        self.assertEqual(median([2, 3, 3, 3, 3, 5]), 3.0)

    def test_6(self):
        self.assertEqual(median([1, 1, 3, 4, 6, 6, 6, 7, 10]), 6)

    def test_7(self):
        self.assertEqual(median([3, 4, 6, 6, 6, 7, 9, 10, 10]), 6)

    def test_8(self):
        self.assertEqual(median([3, 3, 4, 5, 6, 6, 7, 9]), 5.5)

    def test_9(self):
        self.assertEqual(median([3, 4, 4, 6, 9, 9, 9]), 6)

    def test_10(self):
        self.assertEqual(median([3, 4, 4, 5, 7, 8]), 4.5)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Basic Statistics: Median](https://edabit.com/challenge/KqR5XyJSJcJFnD5uF)
