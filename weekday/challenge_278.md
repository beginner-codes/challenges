# Challenge 278 - Ransom Letter

Write a function that returns `True` if you can use the letters of the first string to create the second string. Letters are case-sensitive.

## Examples
```python
can_build("aPPleAL", "PAL") ➞ True

can_build("aPPleAL", "apple") ➞ False

can_build("a", "") ➞ True

can_build("aa", "aaa") ➞ False
```
## Notes

- Letters in the first string can be used only once.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def can_build(letters: str, string: str) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(can_build("aPPleAL", "PAL"))

    def test_2(self):
        self.assertTrue(can_build("OAT", "OAT"))

    def test_3(self):
        self.assertTrue(can_build("maybelLINE", "maybe"))

    def test_4(self):
        self.assertTrue(can_build("topsh", "shop"))

    def test_5(self):
        self.assertTrue(can_build("topshSHP", "SHoP"))

    def test_6(self):
        self.assertTrue(can_build("DAISIES", "SAID"))

    def test_7(self):
        self.assertTrue(can_build("ToporP", "porT"))

    def test_8(self):
        self.assertTrue(can_build("PoTluCK", "PuCK"))

    def test_9(self):
        self.assertTrue(can_build("pATS", "p"))

    def test_10(self):
        self.assertTrue(can_build("blah", ""))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Ransom Letter](https://edabit.com/challenge/EHzL3v25wYp7E4AFC)
