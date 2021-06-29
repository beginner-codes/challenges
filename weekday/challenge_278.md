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

    def test_16(self):
        self.assertFalse(can_build("a", "aA"))

    def test_17(self):
        self.assertFalse(can_build("a", "A"))

    def test_18(self):
        self.assertFalse(can_build("AAAAAA", "AAAAAAa"))

    def test_19(self):
        self.assertFalse(can_build("apple", "appleY"))

    def test_20(self):
        self.assertFalse(can_build("xxYYzZ", "zzZxYxY"))

    def test_21(self):
        self.assertFalse(can_build("abCD", "aBCD"))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Ransom Letter](https://edabit.com/challenge/EHzL3v25wYp7E4AFC)
