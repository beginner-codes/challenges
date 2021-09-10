# Challenge 331 - Binary to Decimal Converter

You are given a list containing eight 1's and 0's. Write a function that takes an 8bit binary number and converts it to decimal.

## Examples
```python
binary_to_decimal([1, 1, 1, 1, 1, 1, 1, 1]) ➞ 255

binary_to_decimal([0, 0, 0, 0, 0, 0, 0, 0]) ➞ 0

binary_to_decimal([1, 0, 1, 1, 1, 1, 0, 0]) ➞ 188
```
## Notes

- Return an integer.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def binary_to_decimal(binary_number: list[int]) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(binary_to_decimal([1, 1, 1, 1, 1, 1, 1, 1]), 255)

    def test_2(self):
        self.assertEqual(binary_to_decimal([0, 0, 0, 0, 0, 0, 0, 0]), 0)

    def test_3(self):
        self.assertEqual(binary_to_decimal([1, 0, 1, 1, 1, 1, 0, 0]), 188)

    def test_4(self):
        self.assertEqual(binary_to_decimal([1, 0, 1, 1, 0, 1, 0, 1]), 181)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Binary to Decimal Converter](https://edabit.com/challenge/xmyWLvzP5df6okDTG)
