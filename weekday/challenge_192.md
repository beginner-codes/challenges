# Challenge 192 - Two Distinct Elements

In each input list, every number repeats at least once, except for two. Write a function that returns the two unique numbers.

## Examples
```python
return_unique([1, 9, 8, 8, 7, 6, 1, 6]) ➞ [9, 7]

return_unique([5, 5, 2, 4, 4, 4, 9, 9, 9, 1]) ➞ [2, 1]

return_unique([9, 5, 6, 8, 7, 7, 1, 1, 1, 1, 1, 9, 8]) ➞ [5, 6]
```
## Notes

- Keep the same ordering in the output.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```py
from __future__ import annotations
import unittest


def return_unique(sequence: list[int]) -> list[int]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(return_unique([1, 9, 8, 8, 7, 6, 1, 6]), [9, 7])

    def test_2(self):
        self.assertEqual(return_unique([5, 5, 2, 4, 4, 4, 9, 9, 9, 1]), [2, 1])

    def test_3(self):
        self.assertEqual(return_unique([9, 5, 6, 8, 7, 7, 1, 1, 1, 1, 1, 9, 8]), [5, 6])

    def test_4(self):
        self.assertEqual(return_unique([4, 3, 9, 9, 1, 1, 6, 1, 6, 2, 4]), [3, 2])

    def test_5(self):
        self.assertEqual(
            return_unique([44, 44, 44, 2, 55, 55, 55, 0, 66, 66, 66]), [2, 0]
        )

    def test_6(self):
        self.assertEqual(return_unique([-9, -9, -9, 7, -9, -9, 1]), [7, 1])

    def test_7(self):
        self.assertEqual(
            return_unique([2, 2, -19, 2, 7, 7, 4, 9, 9, 0, 0, 3, 3, 3]), [-19, 4]
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Two Distinct Elements](https://edabit.com/challenge/yL5WmWTCNwwb4GnR7)
