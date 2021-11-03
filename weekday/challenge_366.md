# Challenge 366 - Accumulating Product

Create a function that takes a list and returns a list of the accumulated products.

## Examples
```python
accumulating_product([1, 2, 3, 4]) ➞ [1, 2, 6, 24]
# [1, 2, 6, 24] can be written as [1, 1 x 2, 1 x 2 x 3, 1 x 2 x 3 x 4]

accumulating_product([1, 5, 7]) ➞ [1, 5, 35]

accumulating_product([1, 0, 1, 0]) ➞ [1, 0, 0, 0]

accumulating_product([]) ➞ []
```
## Notes

- An empty list should return an empty list.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def accumulating_product(numbers: list[int]) -> list[int]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(accumulating_product([1, 2, 3, 4]), [1, 2, 6, 24])

    def test_2(self):
        self.assertListEqual(accumulating_product([5, 10, 1, 1]), [5, 50, 50, 50])

    def test_3(self):
        self.assertListEqual(accumulating_product([1, 5, 7]), [1, 5, 35])

    def test_4(self):
        self.assertListEqual(accumulating_product([1, 0, 1, 0]), [1, 0, 0, 0])

    def test_5(self):
        self.assertListEqual(accumulating_product([1]), [1])

    def test_6(self):
        self.assertListEqual(
            accumulating_product([1, 2, 2, 2, 2, 2, 2]), [1, 2, 4, 8, 16, 32, 64]
        )

    def test_7(self):
        self.assertListEqual(
            accumulating_product([1, 1, 1, 1, 1, 1, 1]), [1, 1, 1, 1, 1, 1, 1]
        )

    def test_8(self):
        self.assertListEqual(accumulating_product([]), [])


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Accumulating Product](https://edabit.com/challenge/iMRN9YGK4mcYja9rY)
