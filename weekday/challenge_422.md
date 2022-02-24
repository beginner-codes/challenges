# Challenge 422 - Positive Dominant

A list is positive dominant if it contains strictly more unique positive values than unique negative values. Write a function that returns `True` if a list is positive dominant.

## Examples
```python
is_positive_dominant([1, 1, 1, 1, -3, -4]) ➞ False
# There is only 1 unique positive value (1).
# There are 2 unique negative values (-3, -4)

is_positive_dominant([5, 99, 832, -3, -4]) ➞ True

is_positive_dominant([5, 0]) ➞ True

is_positive_dominant([0, -4, -1]) ➞ False
```
## Notes

- `0` counts as neither a positive nor a negative value.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def is_positive_dominant(numbers: list[int]) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertFalse(is_positive_dominant([1, 1, 1, 1, -3, -4]))

    def test_2(self):
        self.assertTrue(is_positive_dominant([5, 99, 832, -3, -4]))

    def test_3(self):
        self.assertTrue(is_positive_dominant([5, 0]))

    def test_4(self):
        self.assertFalse(is_positive_dominant([0, -4, -1]))

    def test_5(self):
        self.assertTrue(is_positive_dominant([1, 2, 3, -1]))

    def test_6(self):
        self.assertFalse(is_positive_dominant([1, 0, 0, -1]))

    def test_7(self):
        self.assertTrue(is_positive_dominant([5, 4, 3, 0, 0, -1, -1, -2, -2]))

    def test_8(self):
        self.assertFalse(is_positive_dominant([52, 52, 52, -3, 2, 2, 2, -4]))

    def test_9(self):
        self.assertFalse(is_positive_dominant([3, 3, 3, 3, -1, -1, -1]))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Positive Dominant](https://edabit.com/challenge/eboWapTruZFxmdcwp)
