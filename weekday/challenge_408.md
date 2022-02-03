# Challenge 408 - Next Happy Year

A Happy Year is any year with only distinct digits. Create a function that takes an integer year and returns the next happy year.

## Examples
```python
happy_year(2017) ➞ 2018
# 2018 has all distinct digits

happy_year(1990) ➞ 2013

happy_year(2021) ➞ 2031
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def happy_year(year: int) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(happy_year(1990), 2013)

    def test_2(self):
        self.assertEqual(happy_year(2017), 2018)

    def test_3(self):
        self.assertEqual(happy_year(2021), 2031)

    def test_4(self):
        self.assertEqual(happy_year(1001), 1023)

    def test_5(self):
        self.assertEqual(happy_year(1123), 1203)

    def test_6(self):
        self.assertEqual(happy_year(2001), 2013)

    def test_7(self):
        self.assertEqual(happy_year(2334), 2340)

    def test_8(self):
        self.assertEqual(happy_year(3331), 3401)

    def test_9(self):
        self.assertEqual(happy_year(1987), 2013)

    def test_10(self):
        self.assertEqual(happy_year(5555), 5601)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Next Happy Year](https://edabit.com/challenge/5FoNY2Z7B5wSCDTA4)
