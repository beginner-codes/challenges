# Challenge 219 - Impossible Date

Given the parameters day, month and year, return whether that date is a valid date.

## Examples
```python
is_valid_date(35, 2, 2020) ➞ False
# February doesn't have 35 days.

is_valid_date(8, 3, 2020) ➞ True
# 8th March 2020 is a real date.

is_valid_date(31, 6, 1980) ➞ False
# June only has 30 days.
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def is_valid_date(day: int, month: int, year: int) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertFalse(is_valid_date(35, 2, 2020))

    def test_2(self):
        self.assertTrue(is_valid_date(8, 3, 2020))

    def test_3(self):
        self.assertFalse(is_valid_date(31, 6, 1980))

    def test_4(self):
        self.assertTrue(is_valid_date(27, 9, 1822))

    def test_5(self):
        self.assertFalse(is_valid_date(34, 7, 2008))

    def test_6(self):
        self.assertFalse(is_valid_date(32, 12, 1932))

    def test_7(self):
        self.assertTrue(is_valid_date(20, 3, 2019))

    def test_8(self):
        self.assertTrue(is_valid_date(28, 3, 2004))

    def test_9(self):
        self.assertTrue(is_valid_date(22, 5, 1962))

    def test_10(self):
        self.assertTrue(is_valid_date(21, 11, 1875))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Impossible Date](https://edabit.com/challenge/HnrmZxpGRoPkmZsfs)
