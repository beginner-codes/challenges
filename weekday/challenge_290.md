# Challenge 290 - Construct and Deconstruct

Given a string, create a function that outputs a list, building and deconstructing the string letter by letter. See the examples below for some helpful guidance.

Examples
```python
construct_deconstruct("Hello") ➞ [
  "H",
  "He",
  "Hel",
  "Hell",
  "Hello",
  "Hell",
  "Hel",
  "He",
  "H"
]

construct_deconstruct("edabit") ➞ [
  "e",
  "ed",
  "eda",
  "edab",
  "edabi",
  "edabit",
  "edabi",
  "edab",
  "eda",
  "ed",
  "e"
]

construct_deconstruct("the sun") ➞ [
  "t",
  "th",
  "the",
  "the ",
  "the s",
  "the su",
  "the sun",
  "the su",
  "the s",
  "the ",
  "the",
  "th",
  "t"
]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def construct_deconstruct(string: str) -> list[str]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(
            construct_deconstruct("Hello"),
            ["H", "He", "Hel", "Hell", "Hello", "Hell", "Hel", "He", "H"],
        )

    def test_2(self):
        self.assertListEqual(
            construct_deconstruct("edabit"),
            [
                "e",
                "ed",
                "eda",
                "edab",
                "edabi",
                "edabit",
                "edabi",
                "edab",
                "eda",
                "ed",
                "e",
            ],
        )

    def test_3(self):
        self.assertListEqual(
            construct_deconstruct("the sun"),
            [
                "t",
                "th",
                "the",
                "the ",
                "the s",
                "the su",
                "the sun",
                "the su",
                "the s",
                "the ",
                "the",
                "th",
                "t",
            ],
        )

    def test_8(self):
        self.assertListEqual(construct_deconstruct(""), [])

    def test_9(self):
        self.assertListEqual(
            construct_deconstruct("        "),
            [
                " ",
                "  ",
                "   ",
                "    ",
                "     ",
                "      ",
                "       ",
                "        ",
                "       ",
                "      ",
                "     ",
                "    ",
                "   ",
                "  ",
                " ",
            ],
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Construct and Deconstruct](https://edabit.com/challenge/rwPguhgju54AMR2kM)
