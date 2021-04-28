# Challenge 234 - Palindromic Dates

The 2nd of February 2020 was a palindromic date in both `dd/mm/yyyy` and `mm/dd/yyyy` format (02/02/2020). Given a date in `dd/mm/yyyy` format, return `True` if the date is palindromic in both date formats, otherwise return `False`.

## Examples
```python
palindromic_date("02/02/2020") ➞ True

palindromic_date("11/12/2019") ➞ False

palindromic_date("11/02/2011") ➞ False
# Although 11/02/2011 is palindromic in dd/mm/yyyy format,
# it isn't in mm/dd/yyyy format (02/11/2011)
```
## Notes

- All dates will be valid in both date formats.
- The date must be palindromic in both `dd/mm/yyyy` and `mm/dd/yyyy` formats to pass.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def palindromic_date(date: str) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(palindromic_date("02/02/2020"))

    def test_2(self):
        self.assertFalse(palindromic_date("11/12/2019"))

    def test_3(self):
        self.assertFalse(palindromic_date("11/02/2011"))

    def test_4(self):
        self.assertFalse(palindromic_date("06/10/1469"))

    def test_5(self):
        self.assertFalse(palindromic_date("06/05/3133"))

    def test_6(self):
        self.assertTrue(palindromic_date("12/12/2121"))

    def test_7(self):
        self.assertTrue(palindromic_date("09/09/9090"))

    def test_8(self):
        self.assertFalse(palindromic_date("11/04/2203"))

    def test_9(self):
        self.assertTrue(palindromic_date("07/07/7070"))

    def test_10(self):
        self.assertFalse(palindromic_date("06/11/2923"))

    def test_11(self):
        self.assertFalse(palindromic_date("03/08/8030"))

    def test_12(self):
        self.assertTrue(palindromic_date("01/01/1010"))

    def test_13(self):
        self.assertFalse(palindromic_date("03/11/3369"))

    def test_14(self):
        self.assertFalse(palindromic_date("11/03/2775"))

    def test_15(self):
        self.assertFalse(palindromic_date("03/03/1822"))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Palindromic Dates](https://edabit.com/challenge/Qqd2symFeFe4y5YGG)
