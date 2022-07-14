# Challenge 407 - Sum of Digits Between Two Numbers

Create a function that sums the total number of digits between two numbers, inclusive. For example, between the numbers 19 and 22 we have:
```
# 19, 20, 21, 22
(1 + 9) + (2 + 0) + (2 + 1) + (2 + 2) = 19
```
## Examples
```python
sum_digits(7, 8) ➞ 15

sum_digits(17, 20) ➞ 29

sum_digits(10, 12) ➞ 6
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def sum_digits(number_a: int, number_b: int) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(sum_digits(7, 8), 15)

    def test_2(self):
        self.assertEqual(sum_digits(17, 20), 29)

    def test_3(self):
        self.assertEqual(sum_digits(10, 12), 6)

    def test_4(self):
        self.assertEqual(sum_digits(500, 506), 56)

    def test_5(self):
        self.assertEqual(sum_digits(66, 789), 9324)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Sum of Digits Between Two Numbers](https://edabit.com/challenge/kmruefq3dhdqxtLeM)
