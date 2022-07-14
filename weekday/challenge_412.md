# Challenge 412 - Is the Phone Number Formatted Correctly?

Create a function that accepts a string and returns `True` if it's in the format of a proper phone number and `False` if it's not. Assume any number between `0-9` (in the appropriate spots) will produce a valid phone number.

This is what a valid phone number looks like: `(123) 456-7890`

## Examples
```python
is_valid_phone_number("(123) 456-7890") ➞ True

is_valid_phone_number("1111)555 2345") ➞ False

is_valid_phone_number("098) 123 4567") ➞ False
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def is_valid_phone_number(phone_number: str) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(is_valid_phone_number("(123) 456-7890"))

    def test_2(self):
        self.assertFalse(is_valid_phone_number("(1111)555 2345"))

    def test_3(self):
        self.assertFalse(is_valid_phone_number("(098) 123 4567"))

    def test_4(self):
        self.assertFalse(is_valid_phone_number("(123)456-7890"))

    def test_5(self):
        self.assertFalse(is_valid_phone_number("abc(123)456-7890"))

    def test_6(self):
        self.assertFalse(is_valid_phone_number("(123)456-7890abc"))

    def test_7(self):
        self.assertFalse(is_valid_phone_number("abc(123)456-7890abc"))

    def test_8(self):
        self.assertFalse(is_valid_phone_number("abc(123) 456-7890"))

    def test_9(self):
        self.assertFalse(is_valid_phone_number("(123) 456-7890abc"))

    def test_10(self):
        self.assertFalse(is_valid_phone_number("abc(123) 456-7890abc"))

    def test_11(self):
        self.assertFalse(is_valid_phone_number("(123)-456-7890"))

    def test_12(self):
        self.assertFalse(is_valid_phone_number("(123)_456-7890"))

    def test_13(self):
        self.assertFalse(is_valid_phone_number("-123) 456-7890"))

    def test_14(self):
        self.assertTrue(is_valid_phone_number("(519) 505-6498"))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Is the Phone Number Formatted Correctly?](https://edabit.com/challenge/B2jcSh2RG4GpQYuBz)
