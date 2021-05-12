# Challenge 244 - Oddish vs. Evenish

Create a function that determines whether a number is Oddish or Evenish. A number is Oddish if the sum of all of its digits is odd, and a number is Evenish if the sum of all of its digits is even. If a number is Oddish, return "Oddish". Otherwise, return "Evenish".

For example, `oddish_or_evenish(121)` should return `"Evenish"`, since `1 + 2 + 1 = 4`. `oddish_or_evenish(41)` should return `"Oddish"`, since `4 + 1 = 5`.

## Examples
```python
oddish_or_evenish(43) ➞ "Oddish"
# 4 + 3 = 7
# 7 % 2 = 1

oddish_or_evenish(373) ➞ "Oddish"
# 3 + 7 + 3 = 13
# 13 % 2 = 1

oddish_or_evenish(4433) ➞ "Evenish"
# 4 + 4 + 3 + 3 = 14
# 14 % 2 = 0
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def oddish_or_evenish(number: int) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(oddish_or_evenish(43), "Oddish")

    def test_2(self):
        self.assertEqual(oddish_or_evenish(373), "Oddish")

    def test_3(self):
        self.assertEqual(oddish_or_evenish(55551), "Oddish")

    def test_4(self):
        self.assertEqual(oddish_or_evenish(694), "Oddish")

    def test_5(self):
        self.assertEqual(oddish_or_evenish(4433), "Evenish")

    def test_6(self):
        self.assertEqual(oddish_or_evenish(11), "Evenish")

    def test_7(self):
        self.assertEqual(oddish_or_evenish(211112), "Evenish")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Oddish vs. Evenish](https://edabit.com/challenge/H3t4MkT9wGdL9P6Y3)
