# Challenge 203 - Disarium Number

A number is a Disarium number if the sum of its digits raised to their respective positions is the number itself.

Create a function that determines whether a number is a Disarium number or not.

## Examples
```python
is_disarium(75) ➞ False
# 7^1 + 5^2 = 7 + 25 = 32

is_disarium(135) ➞ True
# 1^1 + 3^2 + 5^3 = 1 + 9 + 125 = 135

is_disarium(544) ➞ False

is_disarium(518) ➞ True

is_disarium(466) ➞ False

is_disarium(8) ➞ True
```
## Notes

- Position of the digit is 1-indexed.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def is_disarium(number: int) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(is_disarium(6), True)

    def test_2(self):
        self.assertEqual(is_disarium(75), False)

    def test_3(self):
        self.assertEqual(is_disarium(135), True)

    def test_4(self):
        self.assertEqual(is_disarium(466), False)

    def test_5(self):
        self.assertEqual(is_disarium(372), False)

    def test_6(self):
        self.assertEqual(is_disarium(175), True)

    def test_7(self):
        self.assertEqual(is_disarium(1), True)

    def test_8(self):
        self.assertEqual(is_disarium(696), False)

    def test_9(self):
        self.assertEqual(is_disarium(876), False)

    def test_10(self):
        self.assertEqual(is_disarium(89), True)

    def test_11(self):
        self.assertEqual(is_disarium(518), True)

    def test_12(self):
        self.assertEqual(is_disarium(598), True)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Disarium Number](https://edabit.com/challenge/yvJbdkmKHvCNtcZy9)
