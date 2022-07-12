# Challenge 316 - Balanced List

Given a list of even length, copy the half with the higher sum of numbers to the other half of the list. If the sum of the first half equals the sum of the second half, return the original list.

## Examples
```python
balanced([1, 2, 4, 6, 3, 1]) ➞ [6, 3, 1, 6, 3, 1]
# 1 + 2 + 4 < 6 + 3 + 1 sol = [6, 3, 1, 6, 3, 1]

balanced([88, 3, 27, 5, 9, 0, 13, 10]) ➞ [88, 3, 27, 5, 88, 3, 27, 5]
# 88 + 3 + 27 + 5 > 9 + 0 + 13 + 10  sol = [88, 3 ,27 ,5 ,88 ,3 ,27 ,5]

balanced([7, 5, 2, 6, 1, 0, 1, 5, 2, 7, 0, 6]) ➞ [7, 5, 2, 6, 1, 0, 1, 5, 2, 7, 0, 6]
# 7 + 5 + 2 + 6 + 1 + 0 = 1 + 5 + 2 + 7 + 0 + 6 sol =  [7, 5, 2, 6, 1, 0, 1, 5, 2, 7, 0, 6]
```
## Notes

- The length of the list is even.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def balanced(lst: list[int]) -> list[int]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(balanced([1, 2, 4, 6, 3, 1]), [6, 3, 1, 6, 3, 1])

    def test_2(self):
        self.assertListEqual(
            balanced([88, 3, 27, 5, 9, 0, 13, 10]), [88, 3, 27, 5, 88, 3, 27, 5]
        )

    def test_3(self):
        self.assertListEqual(
            balanced([7, 5, 2, 6, 1, 0, 1, 5, 2, 7, 0, 6]),
            [7, 5, 2, 6, 1, 0, 1, 5, 2, 7, 0, 6],
        )

    def test_4(self):
        self.assertListEqual(balanced([0, 1, 1, 1]), [1, 1, 1, 1])

    def test_5(self):
        self.assertListEqual(balanced([100, 55]), [100, 100])


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Balanced List](https://edabit.com/challenge/wuQWimjDwkpnd4xJL)
