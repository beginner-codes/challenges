# Challenge 302 - Identity Matrix

An identity matrix is a square matrix with `1`s running from the top left of the square to the bottom right. The rest are `0`s. The identity matrix has applications ranging from machine learning to the theory of relativity.

Create a function that takes an integer and returns the identity matrix of `n x n` dimensions. For this challenge, if the integer is negative, return the mirror image of the identity matrix of `n x n` dimensions. It does not matter if the mirror image is left-right or top-bottom.

## Examples
```python
id_mtrx(2) ➞ [
  [1, 0],
  [0, 1]
]

id_mtrx(-2) ➞ [
  [0, 1],
  [1, 0]
]

id_mtrx(0) ➞ []
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def get_identity_matrix(dimension: int) -> list[list[int]]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(get_identity_matrix(1), [[1]])

    def test_2(self):
        self.assertListEqual(get_identity_matrix(2), [[1, 0], [0, 1]])

    def test_3(self):
        self.assertListEqual(get_identity_matrix(3), [[1, 0, 0], [0, 1, 0], [0, 0, 1]])

    def test_4(self):
        self.assertListEqual(
            get_identity_matrix(4),
            [[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]],
        )

    def test_5(self):
        self.assertListEqual(
            get_identity_matrix(-6),
            [
                [0, 0, 0, 0, 0, 1],
                [0, 0, 0, 0, 1, 0],
                [0, 0, 0, 1, 0, 0],
                [0, 0, 1, 0, 0, 0],
                [0, 1, 0, 0, 0, 0],
                [1, 0, 0, 0, 0, 0],
            ],
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Identity Matrix](https://edabit.com/challenge/QN4RMpAnktNvMCWwg)
