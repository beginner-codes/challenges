# Challenge 297 - Pronic Number

A pronic number (or otherwise called as heteromecic) is a number which is a product of two consecutive integers, that is, a number of the form `n * (n + 1)`. Create a function that determines whether a number is pronic or not.

## Examples
```python
is_heteromecic(0) ➞ True
# 0 * (0 + 1) = 0 * 1 = 0

is_heteromecic(2) ➞ True
# 1 * (1 + 1) = 1 * 2 = 2

is_heteromecic(7) ➞ False

is_heteromecic(110) ➞ True
# 10 * (10 + 1) = 10 * 11 = 110

is_heteromecic(136) ➞ False

is_heteromecic(156) ➞ True
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def is_heteromecic(number: int) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(is_heteromecic(0))

    def test_2(self):
        self.assertTrue(is_heteromecic(2))

    def test_3(self):
        self.assertFalse(is_heteromecic(7))

    def test_4(self):
        self.assertTrue(is_heteromecic(110))

    def test_5(self):
        self.assertFalse(is_heteromecic(136))

    def test_6(self):
        self.assertTrue(is_heteromecic(156))

    def test_7(self):
        self.assertTrue(is_heteromecic(182))

    def test_8(self):
        self.assertFalse(is_heteromecic(218))

    def test_9(self):
        self.assertFalse(is_heteromecic(250))

    def test_10(self):
        self.assertTrue(is_heteromecic(272))


if __name__ == "__main__":
    unittest.main()

```
## Credits

Found on Edabit: [Recursion: Pronic Number](https://edabit.com/challenge/hoxv8zaQJNMWJqnt3)
