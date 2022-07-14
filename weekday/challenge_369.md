# Challenge 369 - Return Duplicate Numbers

Given a list nums where each integer is between 1 and 100, create a function that returns a sorted list containing only duplicate numbers from the given nums list.

## Examples
```python
duplicate_nums([1, 2, 3, 4, 3, 5, 6]) ➞ [3]

duplicate_nums([81, 72, 43, 72, 81, 99, 99, 100, 12, 54]) ➞ [72, 81, 99]

duplicate_nums([1, 2, 3, 4, 5, 6, 7, 8, 9, 10]) ➞ None
```
## Notes

- If there are no duplicate numbers, return None.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def duplicate_nums(nums: list[int]) -> list[int] | None:
    return None  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(duplicate_nums([1, 2, 3, 4, 3, 5, 6]), [3])

    def test_2(self):
        self.assertIsNone(duplicate_nums([1, 2, 3, 4, 5, 6, 7, 8, 9, 10]))

    def test_3(self):
        self.assertListEqual(duplicate_nums([20, 30, 40, 30, 20, 40]), [20, 30, 40])

    def test_4(self):
        self.assertListEqual(
            duplicate_nums([100, 59, 12, 13, 54, 76, 100, 14, 12]), [12, 100]
        )

    def test_5(self):
        self.assertListEqual(
            duplicate_nums([81, 72, 43, 72, 81, 99, 99, 100, 12, 54]), [72, 81, 99]
        )

    def test_6(self):
        self.assertListEqual(
            duplicate_nums([11, 22, 33, 44, 55, 44, 33, 22, 11]), [11, 22, 33, 44]
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Return Duplicate Numbers](https://edabit.com/challenge/c4WKPr4upiKx8GwJK)
