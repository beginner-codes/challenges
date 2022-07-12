# Challenge 417 - Product of Two Largest Numbers

Create a function that takes a list and returns the product of the two largest numbers.

## Examples
```python
product([2, 3, 1, -1, 2]) ➞ 6
# 2 * 3 = 6

product([-2, -2, -1, -1]) ➞ 2
# -2 * - 1 = 2
# Not 1, because you can only use -1 one time.

product([8, 8, 8]) ➞ 64
# 8 * 8 = 64
# You can repeat here because there is only one value.

product([2, 8, 8, 8]) ➞ 16
# 2 * 8 = 16
# Not 64, because you can only use 8 one time.
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def product(numbers: list[int]) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(product([2, 3, 1, -1, 2]), 6)

    def test_2(self):
        self.assertEqual(product([-2, -2, -1, -1]), 2)

    def test_3(self):
        self.assertEqual(product([8, 8, 8]), 64)

    def test_4(self):
        self.assertEqual(product([-2, -1, 100, -12, 0]), 0)

    def test_5(self):
        self.assertEqual(product([1, 2, 3, 4]), 12)

    def test_6(self):
        self.assertEqual(product([-12, 5, 5, 8, 8, 8]), 40)

    def test_7(self):
        self.assertEqual(product([2, 8, 8, 8]), 16)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Product of Two Largest Numbers](https://edabit.com/challenge/T3CDjiW46KT8si6A8)
