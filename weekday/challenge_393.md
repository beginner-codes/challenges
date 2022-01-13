# Challenge 393 - Sum of Missing Numbers

Create a function that returns the sum of the missing numbers.

## Examples
```python
sum_missing_numbers([1, 3, 5, 7, 10]) ➞ 29
# 2 + 4 + 6 + 8 + 9

sum_missing_numbers([10, 7, 5, 3, 1]) ➞ 29

sum_missing_numbers([10, 20, 30, 40, 50, 60]) ➞ 1575
```
## Notes

- The minimum and maximum value of the given list are the inclusive bounds of the numeric range to consider when searching for missing numbers.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def sum_missing_numbers(numbers: list[int]) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(sum_missing_numbers([1, 3, 5, 7, 10]), 29)

    def test_2(self):
        self.assertEqual(sum_missing_numbers([10, 20, 30, 40, 50, 60]), 1575)

    def test_3(self):
        self.assertEqual(sum_missing_numbers([7, 3, 8, 5, 12]), 40)

    def test_4(self):
        self.assertEqual(sum_missing_numbers([99, 2, 45, 4, 17]), 4782)

    def test_5(self):
        self.assertEqual(sum_missing_numbers([10, 7, 5, 3, 1]), 29)

    def test_6(self):
        self.assertEqual(sum_missing_numbers([7, 8, 9, 10]), 0)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Sum of Missing Numbers](https://edabit.com/challenge/e3KZvJbSXeHXtJA7c)
