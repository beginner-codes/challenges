# Challenge 250 - Number of Boomerangs

A boomerang is a V-shaped sequence that is either upright or upside down. Specifically, a boomerang can be defined as: sub-list of length 3, with the first and last digits being the same and the middle digit being different.

Some boomerang examples:
```python
[3, 7, 3], [1, -1, 1], [5, 6, 5]
```
Create a function that returns the total number of boomerangs in a list.

To illustrate:
```python
[3, 7, 3, 2, 1, 5, 1, 2, 2, -2, 2]
# 3 boomerangs in this sequence:  [3, 7, 3], [1, 5, 1], [2, -2, 2]
```
Be aware that boomerangs can overlap, like so:
```python
[1, 7, 1, 7, 1, 7, 1]
# 5 boomerangs (from left to right): [1, 7, 1], [7, 1, 7], [1, 7, 1], [7, 1, 7], and [1, 7, 1]
```
## Examples
```python
count_boomerangs([9, 5, 9, 5, 1, 1, 1]) ➞ 2

count_boomerangs([5, 6, 6, 7, 6, 3, 9]) ➞ 1

count_boomerangs([4, 4, 4, 9, 9, 9, 9]) ➞ 0
```
## Notes

- `[5, 5, 5]` (triple identical digits) is NOT considered a boomerang because the middle digit is identical to the first and last.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def count_boomerangs(boomerangs: list[int]) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(count_boomerangs([9, 5, 9, 5, 1, 1, 1]), 2)

    def test_2(self):
        self.assertEqual(count_boomerangs([5, 6, 6, 7, 6, 3, 9]), 1)

    def test_3(self):
        self.assertEqual(count_boomerangs([4, 4, 4, 9, 9, 9, 9]), 0)

    def test_4(self):
        self.assertEqual(count_boomerangs([5, 9, 5, 9, 5]), 3)

    def test_5(self):
        self.assertEqual(count_boomerangs([4, 4, 4, 8, 4, 8, 4]), 3)

    def test_6(self):
        self.assertEqual(count_boomerangs([2, 2, 2, 2, 2, 2, 3]), 0)

    def test_7(self):
        self.assertEqual(count_boomerangs([2, 2, 2, 2, 3, 2, 3]), 2)

    def test_8(self):
        self.assertEqual(count_boomerangs([1, 2, 1, 1, 1, 2, 1]), 2)

    def test_9(self):
        self.assertEqual(count_boomerangs([5, 1, 1, 1, 1, 4, 1]), 1)

    def test_10(self):
        self.assertEqual(count_boomerangs([3, 7, 3, 2, 1, 5, 1, 2, 2, -2, 2]), 3)

    def test_11(self):
        self.assertEqual(count_boomerangs([1, 7, 1, 7, 1, 7, 1]), 5)

    def test_12(self):
        self.assertEqual(count_boomerangs([5, 5, 5]), 0)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Number of Boomerangs](https://edabit.com/challenge/b7iHQDw72zzkmgCun)
