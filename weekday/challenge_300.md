# Challenge 300 - Perfect Square Patch

Create a function that takes an integer and outputs an `n x n` square solely consisting of the integer `n`.

## Examples
```python
square_patch(3) ➞ [
  [3, 3, 3],
  [3, 3, 3],
  [3, 3, 3]
]

square_patch(5) ➞ [
  [5, 5, 5, 5, 5],
  [5, 5, 5, 5, 5],
  [5, 5, 5, 5, 5],
  [5, 5, 5, 5, 5],
  [5, 5, 5, 5, 5]
]

square_patch(1) ➞ [
  [1]
]

square_patch(0) ➞ []
```
## Notes

- `n` will always be greater than 0.
- If `n` is 0, return an empty list.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def square_patch(n: int) -> list[list[int]]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(square_patch(3), [[3, 3, 3], [3, 3, 3], [3, 3, 3]])

    def test_2(self):
        self.assertListEqual(square_patch(2), [[2, 2], [2, 2]])

    def test_3(self):
        self.assertListEqual(
            square_patch(4), [[4, 4, 4, 4], [4, 4, 4, 4], [4, 4, 4, 4], [4, 4, 4, 4]]
        )

    def test_5(self):
        self.assertListEqual(
            square_patch(5),
            [
                [5, 5, 5, 5, 5],
                [5, 5, 5, 5, 5],
                [5, 5, 5, 5, 5],
                [5, 5, 5, 5, 5],
                [5, 5, 5, 5, 5],
            ],
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Perfect Square Patch](https://edabit.com/challenge/K3qMssK6mF34ctXE5)
