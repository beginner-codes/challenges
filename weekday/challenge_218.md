# Challenge 218 - Pluralize!

Given a list of words in the singular form, return a set of those words in the plural form if they appear more than once in the list.

## Examples
```python
pluralize(["cow", "pig", "cow", "cow"]) ➞ { "cows", "pig" }

pluralize(["table", "table", "table"]) ➞ { "tables" }

pluralize(["chair", "pencil", "arm"]) ➞ { "chair", "pencil", "arm" }
```
## Notes

- This is an oversimplification of the English language so no edge cases will appear.
- Only focus on whether to add an s to the ends of the words.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def min_length(values: list[int], min_value: int) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(min_length([5, 10, 2, -1, 3, 4], 9), 1)

    def test_2(self):
        self.assertEqual(min_length([3, -1, 4, -2, -7, 2], 4), 3)

    def test_3(self):
        self.assertEqual(min_length([-5, 3, 2, 7, 8, 9, -1, 5], 16), 2)

    def test_4(self):
        self.assertEqual(min_length([1, 0, -1, 1, 1], 1), 2)

    def test_5(self):
        self.assertEqual(min_length([1, 0, 1, 1, -1, 0, 1], 2), 4)

    def test_6(self):
        self.assertEqual(min_length([1, 0, 0, 0, 1], 1), 5)

    def test_7(self):
        self.assertEqual(min_length([1, 0, 1, 0, 1], 1), 3)

    def test_8(self):
        self.assertEqual(min_length([-1, 1, 1, 0, 1, 1], 3), 5)

    def test_9(self):
        self.assertEqual(min_length([3, -1, 4, 3, 0, 1, 2], 7), 4)

    def test_10(self):
        self.assertEqual(min_length([0, 1, 1, 0], 2), -1)

    def test_11(self):
        self.assertEqual(min_length([0, 1, 5, 2, 0], 10), -1)

    def test_12(self):
        self.assertEqual(min_length([3, -1, 4, -2, -7, 2], 6), -1)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Shortest Subarray Whose Sum Exceeds N](https://edabit.com/challenge/TmasgxCm6iz3gTGHk)
