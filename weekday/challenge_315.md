# Challenge 315 - In the Centre?

Given a string containing mostly spaces and one non-space character, create a function that returns whether the character is positioned in the very centre of the string. This means the number of spaces on both sides should be the same.

## Examples
```python
is_central("  #  ") ➞ True

is_central(" 2    ") ➞ False

is_central("@") ➞ True
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def is_central(string: str) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(is_central("  #  "))

    def test_2(self):
        self.assertFalse(is_central(" 2    "))

    def test_3(self):
        self.assertTrue(is_central("@"))

    def test_4(self):
        self.assertFalse(is_central(" 1"))

    def test_5(self):
        self.assertFalse(is_central("7 "))

    def test_6(self):
        self.assertFalse(is_central("  l "))

    def test_7(self):
        self.assertFalse(is_central(" a  "))

    def test_8(self):
        self.assertTrue(is_central("    G    "))

    def test_9(self):
        self.assertFalse(is_central("   G     "))

    def test_10(self):
        self.assertTrue(is_central("        %        "))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [In the Centre?](https://edabit.com/challenge/ZrAnDiPTbmrJMHWHD)
