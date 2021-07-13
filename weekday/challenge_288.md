# Challenge 288 - Valid Division

Create a function that takes a division equation d and checks if it will return a whole number without decimals after dividing.

## Examples
```python
valid_division("6/3") ➞ True

valid_division("30/25") ➞ False

valid_division("0/3") ➞ True
```
## Notes

- Return `"invalid"` if division by zero.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from typing import Union
import unittest


def valid_division(equation: str) -> Union[str, bool]:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(valid_division("6/3"))

    def test_2(self):
        self.assertFalse(valid_division("30/25"))

    def test_3(self):
        self.assertTrue(valid_division("0/3"))

    def test_4(self):
        self.assertFalse(valid_division("13/12"))

    def test_5(self):
        self.assertTrue(valid_division("329/329"))

    def test_6(self):
        self.assertTrue(valid_division("20/5"))

    def test_7(self):
        self.assertEqual(valid_division("0/0"), "invalid")

    def test_8(self):
        self.assertEqual(valid_division("10/0"), "invalid")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Valid Division](https://edabit.com/challenge/MTGTSJvAi2iwd2Ygs)
