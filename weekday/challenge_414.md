# Challenge 414 - Spelling Bee

Given a sentence spelling out a word, return `True` if the spelled letters match the word at the end of the string.

## Examples
```python
validate_spelling("C. Y. T. O. P. L. A. S. M. Cytoplasm?") ➞ True

validate_spelling("P. H. A. R. A. O. H. Pharaoh!") ➞ True

validate_spelling("H. A. N. K. E. R. C. H. E. I. F. Handkerchief.") ➞ False
```
## Notes

- The word at the end is always spelled correctly.
- Spelled words will always end in punctuation (but ignore all punctuation).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def validate_spelling(text: str) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(validate_spelling("C. Y. T. O. P. L. A. S. M. Cytoplasm?"))

    def test_2(self):
        self.assertTrue(validate_spelling("P. H. A. R. A. O. H. Pharaoh!"))

    def test_3(self):
        self.assertFalse(validate_spelling("H. A. N. K. E. R. C. H. E. I. F. Handkerchief."))

    def test_4(self):
        self.assertFalse(validate_spelling("M. E. C. O. M. M. E. N. N. Recommend."))

    def test_5(self):
        self.assertTrue(validate_spelling("C. H. R. Y. S. A. N. T. H. E. M. U. M. Chrysanthemum!"))

    def test_6(self):
        self.assertFalse(validate_spelling("A. C. C. O. M. M. O. D. A. M. E. Accommodate!"))

    def test_7(self):
        self.assertFalse(validate_spelling("S. U. A. C. E. I. L. L. A. N. C. E. Surveillance."))

    def test_8(self):
        self.assertTrue(validate_spelling("B. U. S. I. N. E. S. S. Business."))

    def test_9(self):
        self.assertTrue(validate_spelling("C. O. N. V. E. N. I. E. N. T. Convenient."))

    def test_10(self):
        self.assertFalse(validate_spelling("C. O. N. V. E. N. O. E. N. T. Convenient!"))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Spelling Bee](https://edabit.com/challenge/djDJHv3nwWsRM9mtu)
