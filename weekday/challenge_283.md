# Challenge 283 - Sort Positives, Keep Negatives

Write a function that sorts the positive numbers in ascending order, and keeps the negative numbers untouched.

## Examples
```python
pos_neg_sort([6, 3, -2, 5, -8, 2, -2]) ➞ [2, 3, -2, 5, -8, 6, -2]

pos_neg_sort([6, 5, 4, -1, 3, 2, -1, 1]) ➞ [1, 2, 3, -1, 4, 5, -1, 6]

pos_neg_sort([-5, -5, -5, -5, 7, -5]) ➞ [-5, -5, -5, -5, 7, -5]

pos_neg_sort([]) ➞ []
```
## Notes

- If given an empty list, you should return an empty list.
- Integers will always be either positive or negative.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def pos_neg_sort(numbers: list[int]) -> list[int]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(
            pos_neg_sort([6, 3, -2, 5, -8, 2, -2]), [2, 3, -2, 5, -8, 6, -2]
        )

    def test_2(self):
        self.assertListEqual(
            pos_neg_sort([6, 5, 4, -1, 3, 2, -1, 1]), [1, 2, 3, -1, 4, 5, -1, 6]
        )

    def test_3(self):
        self.assertListEqual(
            pos_neg_sort([-5, -5, -5, -5, 7, -5]), [-5, -5, -5, -5, 7, -5]
        )

    def test_4(self):
        self.assertListEqual(
            pos_neg_sort([-5, -5, -5, -5, -4, -5]), [-5, -5, -5, -5, -4, -5]
        )

    def test_5(self):
        self.assertListEqual(
            pos_neg_sort([-5, 4, -8, 3, -1, 2, 1, -7]), [-5, 1, -8, 2, -1, 3, 4, -7]
        )

    def test_6(self):
        self.assertListEqual(pos_neg_sort([-5, 4, 3]), [-5, 3, 4])

    def test_7(self):
        self.assertListEqual(pos_neg_sort([]), [])


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Sort Positives, Keep Negatives](https://edabit.com/challenge/6brSyFwWnb9Msu7kX)
