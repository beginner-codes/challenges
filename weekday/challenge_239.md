# Challenge 239 - Length of Line Segment

Write a function that takes coordinates of two points on a two-dimensional plane and returns the length of the line segment connecting those two points.

## Examples
```python
line_length((15, 7), (22, 11)) ➞ 8.06

line_length((0, 0), (0, 0)) ➞ 0

line_length((0, 0), (1, 1)) ➞ 1.41
```
## Notes

- The order of the given numbers is X, Y.
- This challenge is easier than it looks.
- Round your result to two decimal places.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def line_length(point_a: tuple[int, int], point_b: tuple[int, int]) -> float:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(line_length((15, 7), (22, 11)), 8.06)

    def test_2(self):
        self.assertEqual(line_length((0, 0), (0, 0)), 0)

    def test_3(self):
        self.assertEqual(line_length((0, 0), (1, 1)), 1.41)

    def test_4(self):
        self.assertEqual(line_length((30, 10), (13, -5)), 22.67)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Geometry 1: Length of Line Segment](https://edabit.com/challenge/3Ekam9jvbNKHDtx4K)
