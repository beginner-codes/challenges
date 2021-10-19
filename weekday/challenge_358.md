# Challenge 358 - Sum of Every Nth Number

Given a list of numbers and a positive value for `n`, create a function that returns the sum of every `n`th number in the list.

## Examples
```python
sum_every_nth([4, 8, 6, 6, 7, 9, 3], 1) ➞ 43
# 4+8+6+6+7+9+3 = 43

sum_every_nth([7, 3, 10, 4, 5, 8, 4, 9, 6, 9, 10, 1, 4], 4) ➞ 14
# 4+9+1 = 14

sum_every_nth([10, 6, 5, 4, 5, 2, 3, 3, 8, 10, 7, 2], 8) ➞ 3
# 3

sum_every_nth([6, 8, 9, 4, 6, 4, 7, 1, 5, 6, 10, 2], 13) ➞ 0
# only 12 numbers in list
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def sum_every_nth(numbers: list[int], n: int) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(sum_every_nth([2, 5, 3, 9, 5, 7, 10, 7, 3, 3, 3], 9), 3)

    def test_2(self):
        self.assertEqual(
            sum_every_nth([10, 9, 2, 5, 9, 6, 4, 6, 7, 10, 9, 9, 9, 9, 2, 1, 2], 7), 13
        )

    def test_3(self):
        self.assertEqual(
            sum_every_nth([4, 5, 8, 7, 8, 1, 7, 9, 7, 4, 6, 2, 8, 8, 9, 9, 1, 7, 4], 6),
            10,
        )

    def test_4(self):
        self.assertEqual(
            sum_every_nth(
                [8, 3, 5, 2, 6, 1, 5, 4, 3, 6, 6, 8, 5, 10, 7, 3, 7, 3, 5], 11
            ),
            6,
        )

    def test_5(self):
        self.assertEqual(
            sum_every_nth([8, 9, 4, 8, 7, 5, 2, 9, 1, 8, 3, 8, 4, 9, 9, 6], 11), 3
        )

    def test_6(self):
        self.assertEqual(sum_every_nth([8, 2, 2, 7, 10, 6, 3, 5, 4, 4], 12), 0)

    def test_7(self):
        self.assertEqual(
            sum_every_nth(
                [7, 4, 4, 10, 2, 6, 1, 9, 5, 10, 6, 4, 6, 6, 5, 9, 4, 10, 9], 8
            ),
            18,
        )

    def test_8(self):
        self.assertEqual(
            sum_every_nth(
                [5, 10, 10, 9, 10, 3, 5, 6, 6, 2, 10, 2, 9, 6, 8, 9, 10, 9, 4], 16
            ),
            9,
        )

    def test_9(self):
        self.assertEqual(
            sum_every_nth([10, 4, 8, 4, 3, 9, 1, 1, 10, 7, 1, 4, 5, 5, 6, 1, 9], 6), 13
        )

    def test_10(self):
        self.assertEqual(
            sum_every_nth(
                [2, 6, 3, 10, 6, 5, 4, 7, 9, 4, 1, 8, 9, 10, 8, 7, 2, 3, 6], 8
            ),
            14,
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Sum of Every Nth Number](https://edabit.com/challenge/ET2voBkuSPLb3mFSD)
