# Challenge 217 - Shortest Subarray Whose Sum Exceeds N

Write a function that returns the length of the shortest contiguous sublist whose sum of all elements strictly exceeds `n`.

## Examples
```python
min_length([5, 8, 2, -1, 3, 4], 9) ➞ 2

min_length([3, -1, 4, -2, -7, 2], 4) ➞ 3
# Shortest sublist whose sum exceeds 4 is: [3, -1, 4]

min_length([1, 0, 0, 0, 1], 1) ➞ 5

min_length([0, 1, 1, 0], 2) ➞ -1
```
## Notes

- The sublist should be composed of contiguous elements from the original list.
- If no such sublist exists, return `-1`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def min_length(values: list[int], min_value: int) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(min_length([5, 10, 2, -1, 3, 4], 9), 1)

    def test_2(self):
        self.assertEqual(min_length([3, -1, 4, -2, -7, 2], 4), 3)

    def test_3(self):
        self.assertEqual(min_length([-5, 3, 2, 7, 8, 9, -1, 5], 16), 2)

    def test_4(self):
        self.assertEqual(min_length([1, 0, -1, 1, 1], 1), 2)

    def test_5(self):
        self.assertEqual(min_length([1, 0, 1, 1, -1, 0, 1], 2), 4)

    def test_6(self):
        self.assertEqual(min_length([1, 0, 0, 0, 1], 1), 5)

    def test_7(self):
        self.assertEqual(min_length([1, 0, 1, 0, 1], 1), 3)

    def test_8(self):
        self.assertEqual(min_length([-1, 1, 1, 0, 1, 1], 3), 5)

    def test_9(self):
        self.assertEqual(min_length([3, -1, 4, 3, 0, 1, 2], 7), 4)

    def test_10(self):
        self.assertEqual(min_length([0, 1, 1, 0], 2), -1)

    def test_11(self):
        self.assertEqual(min_length([0, 1, 5, 2, 0], 10), -1)

    def test_12(self):
        self.assertEqual(min_length([3, -1, 4, -2, -7, 2], 6), -1)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Shortest Subarray Whose Sum Exceeds N](https://edabit.com/challenge/TmasgxCm6iz3gTGHk)
