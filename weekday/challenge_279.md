# Challenge 279 - Building up a Word

You are given an input list of strings, ordered by ascending length.

Write a function that returns `True` if, for each pair of consecutive strings, the second string can be formed from the first by adding a single letter either at the beginning or end.

## Examples
```python
can_build(["a", "at", "ate", "late", "plate", "plates"]) ➞ True

can_build(["a", "at", "ate", "late", "plate", "plater", "platter"]) ➞ False
# "platter" is formed by adding "t" in the middle of "plater"

can_build(["it", "bit", "bite", "biters"]) ➞ False
# "biters" is formed by adding two letters - we can only add one

can_build(["mean", "meany"]) ➞ True
```
## Notes

- Return `False` if a word is NOT formed by adding only one letter.
- Return `False` if the letter is added to the middle of the previous word.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def can_build(words: list[str]) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(can_build(["a", "at", "ate", "late", "plate", "plates"]))

    def test_2(self):
        self.assertFalse(can_build(["a", "at", "ate", "late", "plate", "plater", "platter"]))

    def test_3(self):
        self.assertTrue(can_build(["a", "ka", "ika", "pika", "pikac", "pikach", "pikachu"]))

    def test_4(self):
        self.assertFalse(can_build(["e", "tea", "teac", "teach", "teache", "teacher", "teachers"]))

    def test_5(self):
        self.assertTrue(can_build(["a", "at", "tat", "stat", "state", "estate", "estates"]))

    def test_6(self):
        self.assertFalse(can_build(["m", "ma", "man", "many", "meany"]))

    def test_7(self):
        self.assertTrue(can_build(["o", "ol", "old", "bold", "bolde", "mbolde", "embolde", "embolden"]))

    def test_8(self):
        self.assertFalse(can_build(["o", "op", "top", "stop", "stops", "stoops"]))

    def test_9(self):
        self.assertTrue(can_build(["mean", "meany"]))

    def test_10(self):
        self.assertFalse(can_build(["air", "air", "airy", "fairy"]))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Building up a Word](https://edabit.com/challenge/zQespQxTsiGoeMNP3)
