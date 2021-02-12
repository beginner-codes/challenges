# Challenge 182 - Sum Fractions

Create a function that takes series of tuples as arguments. Each tuple has 2 elements. The first element is the numerator and the second element is the denominator. Return the sum of the fractions rounded to the nearest whole number.

## Examples
```python
sum_fractions((18, 13), (4, 5)) ➞ 2

sum_fractions((36, 4), (22, 60)) ➞ 9

sum_fractions((11, 2), (3, 4), (5, 4), (21, 11), (12, 6)) ➞ 11
```
## Notes

- Your result should be a number not string.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```py
from __future__ import annotations
import unittest


def sum_fractions(*fractions: tuple[int, int]) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(sum_fractions((36, 4), (22, 60)), 9)

    def test_2(self):
        self.assertEqual(sum_fractions((-11, 12), (18, 13), (4, 5)), 1)

    def test_3(self):
        self.assertEqual(sum_fractions((11, 12), (18, 13), (4, 5)), 3)

    def test_4(self):
        self.assertEqual(sum_fractions((18, 13), (4, 5)), 2)

    def test_5(self):
        self.assertEqual(sum_fractions((41, 14), (10, 91)), 3)

    def test_6(self):
        self.assertEqual(sum_fractions((11, 2), (3, 4), (5, 4), (21, 11), (12, 6)), 11)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Sum Fractions](https://edabit.com/challenge/qaNmoG4dAXRL5JqvA)
