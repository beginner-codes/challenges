# Challenge 441 - Merge Lists in Order

Given two lists, merge them to one list and sort the new list in the same order as the first list.

## Examples
```python
merge_and_sort([1, 2, 3], [5, 4, 6]) ➞ [1, 2, 3, 4, 5, 6]

merge_and_sort([8, 6, 4, 2], [-2, -6, 0, -4]) ➞ [8, 6, 4, 2, 0, -2, -4, -6]

merge_and_sort([120, 180, 200], [190, 175, 130]) ➞ [120, 130, 175, 180, 190, 200]
```
## Notes

- You'll always get two lists as arguments.
- The first list is always sorted, either asc or desc.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def merge_and_sort(sorted_list: list[int], merge_list: list[int]) -> list[int]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(merge_and_sort([1, 2, 3], [5, 4, 6]), [1, 2, 3, 4, 5, 6])

    def test_2(self):
        self.assertListEqual(merge_and_sort([8, 6, 4, 2], [-2, -6, 0, -4]), [8, 6, 4, 2, 0, -2, -4, -6])

    def test_3(self):
        self.assertListEqual(merge_and_sort([120, 180, 200], [190, 175, 130]), [120, 130, 175, 180, 190, 200])

    def test_4(self):
        self.assertListEqual(merge_and_sort([25, 21, 17, 13], []), [25, 21, 17, 13])

    def test_5(self):
        self.assertListEqual(merge_and_sort([1024, 2048], [512, 128, 64]), [64, 128, 512, 1024, 2048])

    def test_6(self):
        self.assertListEqual(merge_and_sort([0, 1], [1, 1, 1, 1, 0, 0, 0, 0]), [0, 0, 0, 0, 0, 1, 1, 1, 1, 1])

    def test_7(self):
        self.assertListEqual(merge_and_sort([-1, -3], [11, -5, 7, -11]), [11, 7, -1, -3, -5, -11])

    def test_8(self):
        self.assertListEqual(merge_and_sort([10, 20, 30, 40, 50, 60, 80, 90], [70]), [10, 20, 30, 40, 50, 60, 70, 80, 90])


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Merge Lists in Order](https://edabit.com/challenge/zxAXEgpjQ3XrLs2K7)
