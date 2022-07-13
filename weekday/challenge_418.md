# Challenge 418 - Delete Occurrences of Extra Elements in a List

Create a function that takes two arguments: a list of items and a number. If an element occurs in the list more than that number of times, remove the extra occurrences and return the resulting list.

## Examples
```python
delete_occurrences([1, 1, 1, 1], 2) ➞ [1, 1]

delete_occurrences([13, True, 13, None], 1) ➞ [13, True, None]

delete_occurrences([True, True, True], 3) ➞ [True, True, True]
```
## Notes

- Do not alter the order of the original list.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from typing import Any
import unittest


def delete_occurrences(items: list[Any], limit: int) -> list[Any]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(delete_occurrences([1, 1, 1, 1], 2), [1, 1])

    def test_2(self):
        self.assertListEqual(
            delete_occurrences([True, True, True], 3), [True, True, True]
        )

    def test_3(self):
        self.assertListEqual(
            delete_occurrences([13, True, 13, None], 1), [13, True, None]
        )

    def test_4(self):
        self.assertListEqual(delete_occurrences([], 100), [])

    def test_5(self):
        self.assertListEqual(
            delete_occurrences(["John", "John", "Marry", "Marry"], 1), ["John", "Marry"]
        )

    def test_6(self):
        self.assertListEqual(delete_occurrences([20, 37, 20, 21], 1), [20, 37, 21])

    def test_7(self):
        self.assertListEqual(
            delete_occurrences([1, 1, 3, 3, 7, 2, 2, 2, 2], 3), [1, 1, 3, 3, 7, 2, 2, 2]
        )

    def test_8(self):
        self.assertListEqual(
            delete_occurrences([1, 2, 3, 1, 1, 2, 1, 2, 3, 3, 2, 4, 5, 3, 1], 3),
            [1, 2, 3, 1, 1, 2, 2, 3, 3, 4, 5],
        )

if __name__ == "__main__":
    unittest.main()

```
## Credits

Found on Edabit: [Delete Occurrences of Extra Elements in a List](https://edabit.com/challenge/iA5aeTFGLcxx94Wjh)
