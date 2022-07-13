# Challenge 439 - Initialize

Create a function that takes in a list of full names and returns the initials.

## Examples
```python
initialize(["Stephen Hawking"]) ➞ ["S. H."]

initialize(["Harry Potter", "Ron Weasley"]) ➞ ["H. P.", "R. W."]

initialize(["Sherlock Holmes", "John Watson", "Irene Adler"]) ➞ ["S. H.", "J. W.", "I. A."]
```
## Notes

- Each initial is followed by a dot.
- Names will always be made of two words, separated by a space.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def initialize(names: list[str]) -> list[str]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(
            initialize(["Sherlock Holmes", "John Watson", "Irene Adler"]),
            ["S. H.", "J. W.", "I. A."],
        )

    def test_2(self):
        self.assertListEqual(
            initialize(["Harry Potter", "Ron Weasley"]), ["H. P.", "R. W."]
        )

    def test_3(self):
        self.assertListEqual(initialize(["Stephen Hawking"]), ["S. H."])

    def test_4(self):
        self.assertListEqual(initialize(["Atticus Finch"]), ["A. F."])

    def test_5(self):
        self.assertListEqual(initialize(["Leonardo DiCaprio"]), ["L. D."])


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Initialize](https://edabit.com/challenge/ANsubgd5zPGxov3u8)
