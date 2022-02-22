# Challenge 420 - Bound Sort

Create a function that returns `True` if an input list can be completely sorted by only sorting within the bounds `[0, n]` (inclusive), where `n` is smaller than or equal to the list's length, and `False` otherwise.

## Examples
```python
bound_sort([1, 6, 5, 3, 8, 9], [0, 3]) ➞ True
# If [1, 6, 5, 3] is sorted to [1, 3, 5, 6], the array is completely sorted.

bound_sort([1, 6, 5, 3, 8, 9], [0, 2]) ➞ False
# Even if [1, 6, 5] is sorted to [1, 5, 6], the array is still not completely sorted.

bound_sort([1, 9, 2, 5, 7], [0, 4]) ➞ True

bound_sort([1, 9, 2, 5, 7], [0, 3]) ➞ False
# Sorting from [0, 3] gives us [1, 2, 5, 9, 7], array still not completely sorted.
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def bound_sort(lst: list[int], bounds: list[int]) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(bound_sort([1, 6, 5, 3, 8, 9], [0, 3]))

    def test_2(self):
        self.assertFalse(bound_sort([1, 6, 5, 3, 8, 9], [0, 2]))

    def test_3(self):
        self.assertTrue(bound_sort([1, 9, 2, 5, 7], [0, 4]))

    def test_4(self):
        self.assertFalse(bound_sort([1, 9, 2, 5, 7], [0, 3]))

    def test_5(self):
        self.assertTrue(bound_sort([1, 2, 3, 4, 5, 8, 9], [0, 1]))

    def test_6(self):
        self.assertTrue(bound_sort([1, 2, 3, 5, 4, 8, 9], [0, 4]))

    def test_7(self):
        self.assertFalse(bound_sort([1, 2, 3, 5, 4, 8, 9], [0, 3]))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Bound Sort](https://edabit.com/challenge/o9jhv8LxsL8KsGgga)
