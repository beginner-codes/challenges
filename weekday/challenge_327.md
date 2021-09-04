# Challenge 327 - Perfect Number

Create a function that tests whether an integer is a perfect number. A perfect number is any number that can be written as the sum of its factors, excluding the number itself.

For example, `6` is a perfect number, since `1 + 2 + 3 = 6`, where `1`, `2`, and `3  are all factors of `6`. Similarly, `28` is a perfect number, since `1 + 2 + 4 + 7 + 14 = 28`.

## Examples
```python
check_perfect(6) ➞ True

check_perfect(28) ➞ True

check_perfect(496) ➞ True

check_perfect(12) ➞ False

check_perfect(97) ➞ False
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def check_perfect(number: int) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(check_perfect(6))

    def test_2(self):
        self.assertTrue(check_perfect(28))

    def test_3(self):
        self.assertTrue(check_perfect(496))

    def test_4(self):
        self.assertTrue(check_perfect(8128))

    def test_5(self):
        self.assertTrue(check_perfect(33550336))

    def test_6(self):
        self.assertFalse(check_perfect(12))

    def test_7(self):
        self.assertFalse(check_perfect(97))

    def test_8(self):
        self.assertFalse(check_perfect(481))

    def test_9(self):
        self.assertFalse(check_perfect(1001))

    def test_10(self):
        self.assertFalse(check_perfect(55555))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Perfect Number](https://edabit.com/challenge/FJ8SmixDM6z3epzGy)
