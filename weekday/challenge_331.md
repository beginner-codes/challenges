# Challenge 332 - Splitting Up Numbers

Create a function that takes a number and returns each place value in the number as a list.

## Examples
```python
num_split(39) ➞ [30, 9]

num_split(-434) ➞ [-400, -30, -4]

num_split(100) ➞ [100, 0, 0]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def num_split(number: int) -> list[int]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(num_split(39), [30, 9])

    def test_2(self):
        self.assertListEqual(num_split(-434), [-400, -30, -4])

    def test_3(self):
        self.assertListEqual(num_split(100), [100, 0, 0])

    def test_4(self):
        self.assertListEqual(num_split(3929), [3000, 900, 20, 9])

    def test_5(self):
        self.assertListEqual(num_split(10293), [10000, 0, 200, 90, 3])

    def test_6(self):
        self.assertListEqual(num_split(900), [900, 0, 0])

    def test_7(self):
        self.assertListEqual(num_split(-100), [-100, 0, 0])


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Splitting Up Numbers](https://edabit.com/challenge/Wd9cCvFKC3fHzgqSx)
