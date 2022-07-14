# Challenge 323 - Number of Times a Character Appears

Create a function that returns the number of times a character appears in each word in a sentence. Treat upper and lower case characters of the same letter as being identical (e.g. `a` exists in `Anna` twice, not once).

## Examples
```python
char_appears("She sells sea shells by the seashore.", "s")
➞ [1, 2, 1, 2, 0, 0, 2]
# "s" shows up once in "She", twice in "sells", once in "sea", twice in "shells", etc.

char_appears("Peter Piper picked a peck of pickled peppers.", "P")
➞ [1, 2, 1, 0, 1, 0, 1, 3]
# "p" shows up once in "Peter", ... 3 times in "peppers".

char_appears("She hiked in the morning, then swam in the river.", "t")
➞ [0, 0, 0, 1, 0, 1, 0, 0, 1, 0]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def char_appears(string: str, search_for: str) -> list[int]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(
            char_appears("She sells sea shells by the seashore.", "s"),
            [1, 2, 1, 2, 0, 0, 2],
        )

    def test_2(self):
        self.assertListEqual(
            char_appears("Peter Piper picked a peck of pickled peppers.", "p"),
            [1, 2, 1, 0, 1, 0, 1, 3],
        )

    def test_3(self):
        self.assertListEqual(
            char_appears("She hiked in the morning, then swam in the river.", "t"),
            [0, 0, 0, 1, 0, 1, 0, 0, 1, 0],
        )

    def test_4(self):
        self.assertListEqual(
            char_appears("I scream, you scream, we all scream for ice cream.", "f"),
            [0, 0, 0, 0, 0, 0, 0, 1, 0, 0],
        )

    def test_5(self):
        self.assertListEqual(char_appears("Snap, crackle, pop!", "p"), [1, 0, 2])

    def test_6(self):
        self.assertListEqual(char_appears("What a wonderful world.", "w"), [1, 0, 1, 1])


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Number of Times a Character Appears](https://edabit.com/challenge/ucsJxQNrkYnpzPaFj)
