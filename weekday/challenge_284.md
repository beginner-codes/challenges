# Challenge 284 - Replace With Next Largest Number

Write a function that replaces each integer with the next largest in the list.

## Examples
```python
replace_next_largest([5, 7, 3, 2, 8]) ➞ [7, 8, 5, 3, -1]

replace_next_largest([2, 3, 4, 5]) ➞ [3, 4, 5, -1]

replace_next_largest([1, 0, -1, 8, -72]) ➞ [8, 1, 0, -1, -1]
```
## Notes

- Replace the maximum with `-1`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def replace_next_largest(numbers: list[int]) -> list[int]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(replace_next_largest([5, 7, 3, 2, 8]), [7, 8, 5, 3, -1])

    def test_2(self):
        self.assertListEqual(
            replace_next_largest([4, 1, 6, -7, -8, 2]), [6, 2, -1, 1, -7, 4]
        )

    def test_3(self):
        self.assertListEqual(replace_next_largest([2, 3, 4, 5]), [3, 4, 5, -1])

    def test_4(self):
        self.assertListEqual(
            replace_next_largest([1, 0, -1, 8, -72]), [8, 1, 0, -1, -1]
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Replace With Next Largest Number](https://edabit.com/challenge/rgZmbyYh2MSHTX3K6)
