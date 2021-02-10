# Challenge 181 - Sastry Numbers

In this challenge, you have to establish if a given integer `n` is a Sastry number. If the number resulting from the concatenation of an integer `n` with its successor is a perfect square, then `n` is a Sastry Number.

Given a positive integer `n`, implement a function that returns `True` if `n` is a Sastry number, or `False` if it's not.

## Examples
```py
is_sastry(183) ➞ True
# Concatenation of n and its successor = 183184
# 183184 is a perfect square (428 ^ 2)

is_sastry(184) ➞ False
# Concatenation of n and its successor = 184185
# 184185 is not a perfect square

is_sastry(106755) ➞ True
# Concatenation of n and its successor = 106755106756
# 106755106756 is a perfect square (326734 ^ 2)
```
## Notes

- A perfect square is a number with an integer square root.
- You can expect only valid positive integers greater than `0` as input, without exceptions to handle. Zero is a perfect square, but the concatenation `00` isn't considered as a valid result to check.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```py
import unittest


def is_sastry(number: int) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(is_sastry(183))

    def test_2(self):
        self.assertFalse(is_sastry(184))

    def test_3(self):
        self.assertTrue(is_sastry(106755))

    def test_4(self):
        self.assertFalse(is_sastry(129987253440921))

    def test_5(self):
        self.assertTrue(is_sastry(157175907513603))

    def test_6(self):
        self.assertTrue(is_sastry(206611570247935))

    def test_7(self):
        self.assertFalse(is_sastry(338752188230098))

    def test_8(self):
        self.assertTrue(is_sastry(433610247875715))

    def test_9(self):
        self.assertFalse(is_sastry(652333983478884))

    def test_10(self):
        self.assertTrue(is_sastry(718717107443715))

    def test_11(self):
        self.assertFalse(is_sastry(752199872453889))

    def test_12(self):
        self.assertTrue(is_sastry(786704531939448))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Sastry Numbers](https://edabit.com/challenge/JiLom4d6aBk7wAJcZ)
