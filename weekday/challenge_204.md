# Challenge 204 - C*ns*r*d Str*ngs

Someone has attempted to censor my strings by replacing every vowel with a `*`, `l*k* th*s`. Luckily, I've been able to find the vowels that were removed.

Given a censored string and a string of the censored vowels, return the original uncensored string.

## Example
```python
uncensor("Wh*r* d*d my v*w*ls g*?", "eeioeo") ➞ "Where did my vowels go?"

uncensor("abcd", "") ➞ "abcd"

uncensor("*PP*RC*S*", "UEAE") ➞ "UPPERCASE"
```
## Notes

- The vowels are given in the correct order.
- The number of vowels will match the number of * characters in the censored string.

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
