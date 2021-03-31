# Challenge 215 - New Word Builder

Create a function that builds a word from the scrambled letters contained in the first list. Use the second list to establish each position of the letters in the first list. Return a string from the unscrambled letters (that made-up the word).

## Examples
```python
word_builder(["g", "e", "o"], [1, 0, 2]) ➞ "ego"

word_builder(["e", "t", "s", "t"], [3, 0, 2, 1]) ➞ "test"

word_builder(['e', 'i', 'y', 'n', 'r', 'e', 'g', 'n', '.', 'p', 'b'], [10, 0, 6, 1, 3, 7, 5, 4, 8, 9, 2]) ➞ "beginner.py"
```
## Notes

- The elements in the second list are indexes of the elements in the first list.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def word_builder(scambled: list[str], corrected_indexes: list[int]) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(word_builder(["g", "e", "o"], [1, 0, 2]), "ego")

    def test_2(self):
        self.assertEqual(word_builder(["e", "t", "s", "t"], [3, 0, 2, 1]), "test")

    def test_3(self):
        self.assertEqual(
            word_builder(
                ["e", "i", "y", "n", "r", "e", "g", "n", ".", "p", "b"],
                [10, 0, 6, 1, 3, 7, 5, 4, 8, 9, 2],
            ),
            "beginner.py",
        )

    def test_4(self):
        self.assertEqual(
            word_builder(
                ["l", "e", "h", "n", "l", "c", "a", "e", "g"],
                [5, 2, 6, 4, 0, 1, 3, 8, 7],
            ),
            "challenge",
        )

    def test_5(self):
        self.assertEqual(
            word_builder(["s", "o", "r", "t", "e", "d"], [0, 1, 2, 3, 4, 5]), "sorted"
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [New Word Builder](https://edabit.com/challenge/R5F99DeuhqYxbGyMM)
