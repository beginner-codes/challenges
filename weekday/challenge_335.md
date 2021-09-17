# Challenge 335 - Check if a String is a Mathematical Expression

Create a function that takes an input (e.g. `"5 + 4"`) and returns `True` if it's a mathematical expression or `False` if not.

## Examples
```python
math_expr("4 + 5") ➞ True

math_expr("4*6") ➞ True

math_expr("4*no") ➞ False
```
## Notes

- Should only work with the following operations: `+`, `-`, `*`, `/`, `%`
- You don't need to test for floats

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def math_expr(string: str) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(math_expr("5+4"))

    def test_2(self):
        self.assertTrue(math_expr("4 * 5"))

    def test_3(self):
        self.assertTrue(math_expr("3*6"))

    def test_4(self):
        self.assertTrue(math_expr("4 - 5"))

    def test_5(self):
        self.assertTrue(math_expr("6 % 7"))

    def test_6(self):
        self.assertFalse(math_expr("a - b"))

    def test_7(self):
        self.assertFalse(math_expr("a - 2"))

    def test_8(self):
        self.assertFalse(math_expr("nope"))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Check if a String is a Mathematical Expression](https://edabit.com/challenge/hgjdb2nm4ZwuCjtHE)
