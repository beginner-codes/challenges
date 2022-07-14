# Challenge 275 - Puzzle Pieces

Write a function that takes two lists and adds the first element in the first list with the first element in the second list, the second element in the first list with the second element in the second list, etc, etc. Return `True` if all element combinations add up to the same number. Otherwise, return `False`.

## Examples
```python
puzzle_pieces([1, 2, 3, 4], [4, 3, 2, 1]) ➞ True
# 1 + 4 = 5;  2 + 3 = 5;  3 + 2 = 5;  4 + 1 = 5
# Both lists sum to [5, 5, 5, 5]

puzzle_pieces([1, 8, 5, 0, -1, 7], [0, -7, -4, 1, 2, -6]) ➞ True

puzzle_pieces([1, 2], [-1, -1]) ➞ False

puzzle_pieces([9, 8, 7], [7, 8, 9, 10]) ➞ False
```
## Notes

- Each list will have at least one element.
- Return False if both lists are of different length.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def puzzle_pieces(list_a: list[int], list_b: list[int]) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(puzzle_pieces([1, 2, 3, 4], [4, 3, 2, 1]))

    def test_2(self):
        self.assertTrue(puzzle_pieces([1, 8, 5, 0, -1, 7], [0, -7, -4, 1, 2, -6]))

    def test_3(self):
        self.assertTrue(puzzle_pieces([2, 1, 1], [-2, -1, -1]))

    def test_4(self):
        self.assertTrue(puzzle_pieces([2], [-2]))

    def test_5(self):
        self.assertTrue(puzzle_pieces([5, -1], [-6, 0]))

    def test_6(self):
        self.assertTrue(puzzle_pieces([0, 0, 0, 0, 0], [1, 1, 1, 1, 1]))

    def test_7(self):
        self.assertFalse(puzzle_pieces([1, 2], [-1, -1]))

    def test_8(self):
        self.assertFalse(puzzle_pieces([9, 8, 7], [7, 8, 9, 10]))

    def test_9(self):
        self.assertFalse(puzzle_pieces([9, 8, 7], [7, 8, 9, 16]))

    def test_10(self):
        self.assertFalse(puzzle_pieces([1, 1, 1], [1, 1, 2]))

    def test_11(self):
        self.assertFalse(puzzle_pieces([1, 8, 1], [1, -8, -1]))

    def test_12(self):
        self.assertFalse(puzzle_pieces([0, 0, 0, 0, 0], [1, 1, 0, 1, 1]))

    def test_13(self):
        self.assertFalse(puzzle_pieces([0, 0, 0, 0, 0], [1, 1, 1, 1]))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Puzzle Pieces](https://edabit.com/challenge/izfXy5SGfeekmKExH)
