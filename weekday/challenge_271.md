# Challenge 271 - Total Volume of All Boxes

Given a series of boxes, create a function that returns the sum total volume of all those boxes. A box is represented by a list of three integers: length, width and height.

For instance, `total_volume([2, 3, 2], [6, 6, 7], [1, 2, 1])` should return 266 since `(2 x 3 x 2) + (6 x 6 x 7) + (1 x 2 x 1) = 12 + 252 + 2 = 266`.

## Examples
```python
total_volume([4, 2, 4], [3, 3, 3], [1, 1, 2], [2, 1, 1]) ➞ 63

total_volume([2, 2, 2], [2, 1, 1]) ➞ 10

total_volume([1, 1, 1]) ➞ 1
```
## Notes

- You will be given at least one box.
- Each box will always have three dimensions included.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def total_volume(*boxes: list[int]) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(total_volume([4, 2, 4], [3, 3, 3], [1, 1, 2], [2, 1, 1]), 63)

    def test_2(self):
        self.assertEqual(total_volume([2, 2, 2], [2, 1, 1]), 10)

    def test_3(self):
        self.assertEqual(total_volume([1, 1, 1]), 1)

    def test_4(self):
        self.assertEqual(total_volume([5, 1, 10], [1, 9, 2]), 68)

    def test_5(self):
        self.assertEqual(total_volume([1, 1, 5], [3, 3, 1]), 14)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Total Volume of All Boxes](https://edabit.com/challenge/Dq8kbbsLYyG9are5Z)
