# Challenge 276 - Abbreviations Unique?

You are given two inputs:

- A list of abbreviations.
- A list of words.

Write a function that returns `True` if each abbreviation uniquely identifies a word, and `False` otherwise.

## Examples
```python
unique_abbreviations(["ho", "h", "ha"], ["house", "hope", "happy"]) ➞ False
# "ho" and "h" are ambiguous and can identify either "house" or "hope"

unique_abbreviations(["s", "t", "v"], ["stamina", "television", "vindaloo"]) ➞ True

unique_abbreviations(["bi", "ba", "bat"], ["big", "bard", "battery"]) ➞ False

unique_abbreviations(["mo", "ma", "me"], ["moment", "many", "mean"]) ➞ True
```
## Notes

- Abbreviations will be a substring from `[0, n]` from the original string.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def unique_abbreviations(abbreviations: list[str], words: list[str]) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(
            unique_abbreviations(["s", "t", "v"], ["stamina", "television", "vindaloo"])
        )

    def test_2(self):
        self.assertTrue(
            unique_abbreviations(["mo", "ma", "me"], ["moment", "many", "mean"])
        )

    def test_3(self):
        self.assertTrue(
            unique_abbreviations(["at", "o", "abe"], ["atom", "original", "abet"])
        )

    def test_4(self):
        self.assertTrue(
            unique_abbreviations(["rh", "par", "re"], ["rhino", "parry", "residue"])
        )

    def test_5(self):
        self.assertFalse(
            unique_abbreviations(["ho", "h", "ha"], ["house", "hope", "happy"])
        )

    def test_6(self):
        self.assertFalse(
            unique_abbreviations(["bi", "ba", "bat"], ["big", "bard", "battery"])
        )

    def test_7(self):
        self.assertFalse(
            unique_abbreviations(["b", "c", "ch"], ["broth", "chap", "cardigan"])
        )

    def test_8(self):
        self.assertFalse(
            unique_abbreviations(["to", "too", "t"], ["topology", "took", "torrent"])
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Abbreviations Unique?](https://edabit.com/challenge/tjMNAEgkNvM5eyEqJ)
