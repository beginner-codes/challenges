# Challenge 215 - New Word Builder

Create a function that builds a word from the scrambled letters contained in the first list. Use the second list to establish each position of the letters in the first list. Return a string from the unscrambled letters (that made-up the word).

## Examples
```python
word_builder(["g", "e", "o"], [1, 0, 2]) ➞ "ego"

word_builder(["e", "t", "s", "t"], [3, 0, 2, 1]) ➞ "test"

word_builder(["e", "n", "g", "p", "r", "y", ".", "e", "n", "i", "b"], [1, 4, 2, 9, 7, 10, 8, 6, 5, 3, 0]) ➞ "beginner.py"
```
## Notes

- The elements in the second list are indexes of the elements in the first list.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def find_fulcrum(numbers: list[int]) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(find_fulcrum([1, 2, 4, 9, 10, -10, -9, 3]), 4)

    def test_2(self):
        self.assertEqual(find_fulcrum([9, 1, 9]), 1)

    def test_3(self):
        self.assertEqual(find_fulcrum([7, -1, 0, -1, 1, 1, 2, 3]), 0)

    def test_4(self):
        self.assertEqual(find_fulcrum([8, 8, 8, 8]), -1)

    def test_5(self):
        self.assertEqual(find_fulcrum([9, 3, 4, 8, 1]), -1)

    def test_6(self):
        self.assertEqual(find_fulcrum([1, -1, 10, 5, -4, -1]), 10)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [New Word Builder](https://edabit.com/challenge/R5F99DeuhqYxbGyMM)
