# Challenge 314 - Pandigital Numbers

A pandigital number contains all digits (0-9) at least once. Write a function that takes an integer, returning `True` if the integer is pandigital, and `False` otherwise.

## Examples
```python
is_pandigital(98140723568910) ➞ True

is_pandigital(90864523148909) ➞ False
# 7 is missing.

is_pandigital(112233445566778899) ➞ False
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def is_pandigital(number: int) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(is_pandigital(123456789876543210))

    def test_2(self):
        self.assertFalse(is_pandigital(546732965015))

    def test_3(self):
        self.assertTrue(is_pandigital(6781235184590))

    def test_4(self):
        self.assertTrue(is_pandigital(9432821089765))

    def test_5(self):
        self.assertFalse(is_pandigital(678798215643817))

    def test_6(self):
        self.assertFalse(is_pandigital(90864523148909))

    def test_7(self):
        self.assertFalse(is_pandigital(112233445566778899))

    def test_8(self):
        self.assertFalse(is_pandigital(647380265483206))

    def test_9(self):
        self.assertTrue(is_pandigital(38165975424790))

    def test_10(self):
        self.assertFalse(is_pandigital(8146327815320))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Pandigital Numbers](https://edabit.com/challenge/x44ZRvQtJ6TyZQhwx)
