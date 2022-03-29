# Challenge 436 - List Chunking

Given a list and chunk size, create a function such that divides the list into sublists with a length of the given size.

## Examples
```python
chunk([1, 2, 3, 4], 2) ➞ [
  [1, 2], [3, 4]
]

chunk([1, 2, 3, 4, 5, 6, 7], 3) ➞ [
  [1, 2, 3], [4, 5, 6], [7]
]

chunk([1, 2, 3, 4 ,5], 10) ➞ [
  [1, 2, 3, 4, 5]
]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def chunk(numbers: list[int], size: int) -> list[list[int]]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(chunk([1, 2, 3, 4], 2), [[1, 2], [3, 4]])

    def test_2(self):
        self.assertListEqual(chunk([1, 2, 3, 4, 5], 2), [[1, 2], [3, 4], [5]])

    def test_3(self):
        self.assertListEqual(
            chunk([1, 2, 3, 4, 5, 6, 7, 8], 3), [[1, 2, 3], [4, 5, 6], [7, 8]]
        )

    def test_4(self):
        self.assertListEqual(chunk([1, 2, 3, 4, 5], 4), [[1, 2, 3, 4], [5]])

    def test_5(self):
        self.assertListEqual(chunk([1, 2, 3, 4, 5], 10), [[1, 2, 3, 4, 5]])


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [List Chunking](https://edabit.com/challenge/T2G9LR2qNw4rFNu9t)
