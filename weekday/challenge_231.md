# Challenge 231 - Advanced List Sort

Create a function that takes a list of numbers or strings and returns a list with the items from the original list stored into sub-lists. Items of the same value should be in the same sub-list.

## Examples
```python
advanced_sort([2, 1, 2, 1]) ➞ [[2, 2], [1, 1]]

advanced_sort([5, 4, 5, 5, 4, 3]) ➞ [[5, 5, 5], [4, 4], [3]]

advanced_sort(["b", "a", "b", "a", "c"]) ➞ [["b", "b"], ["a", "a"], ["c"]]
```
## Notes

- The sub-lists should be returned in the same order of each element's first appearance in the list.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from typing import TypeVar
import unittest


T = TypeVar("T")


def advanced_sort(lst: list[T]) -> list[list[T]]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(advanced_sort([1, 2, 1, 2]), [[1, 1], [2, 2]])

    def test_2(self):
        self.assertEqual(advanced_sort([2, 1, 2, 1]), [[2, 2], [1, 1]])

    def test_3(self):
        self.assertEqual(advanced_sort([3, 2, 1, 3, 2, 1]), [[3, 3], [2, 2], [1, 1]])

    def test_4(self):
        self.assertEqual(advanced_sort([5, 5, 4, 3, 4, 4]), [[5, 5], [4, 4, 4], [3]])

    def test_5(self):
        self.assertEqual(
            advanced_sort([80, 80, 4, 60, 60, 3]), [[80, 80], [4], [60, 60], [3]]
        )

    def test_6(self):
        self.assertEqual(
            advanced_sort(["c", "c", "b", "c", "b", 1, 1]),
            [["c", "c", "c"], ["b", "b"], [1, 1]],
        )

    def test_7(self):
        self.assertEqual(
            advanced_sort([1234, 1235, 1234, 1235, 1236, 1235]),
            [[1234, 1234], [1235, 1235, 1235], [1236]],
        )

    def test_8(self):
        self.assertEqual(
            advanced_sort(["1234", "1235", "1234", "1235", "1236", "1235"]),
            [["1234", "1234"], ["1235", "1235", "1235"], ["1236"]],
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Advanced List Sort](https://edabit.com/challenge/6vSZmN66xhMRDX8YT)
