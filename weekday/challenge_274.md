# Challenge 274 - Retrieve the Last N Items

Write a function that retrieves the last `n` items from a list.

## Examples
```python
last([1, 2, 3, 4, 5], 1) ➞ [5]

last([4, 3, 9, 9, 7, 6], 3) ➞ [9, 7, 6]

last([1, 2, 3, 4, 5], 7) ➞ "invalid"

last([1, 2, 3, 4, 5], 0) ➞ []
```
## Notes

- Return `"invalid"` if `n` exceeds the length of the list.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from typing import Union
import unittest


def last(lst: list[int], n: int) -> Union[list[int], str]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(last([1, 2, 3, 4, 5], 0), [])

    def test_2(self):
        self.assertEqual(last([1, 2, 3, 4, 5], 1), [5])

    def test_3(self):
        self.assertEqual(last([4, 3, 9, 9, 7, 6], 3), [9, 7, 6])

    def test_4(self):
        self.assertEqual(last([5, 1, 2], 3), [5, 1, 2])

    def test_5(self):
        self.assertEqual(last([], 1), "invalid")

    def test_6(self):
        self.assertEqual(last([1, 2, 3, 4, 5], 7), "invalid")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Retrieve the Last N Elements](https://edabit.com/challenge/HBKAGJZ62JkCTgYX3)
