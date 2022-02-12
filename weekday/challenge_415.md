# Challenge 415 - Letter Distance

Given two words, the letter distance is calculated by taking the absolute value of the difference in character codes and summing up the difference.

If one word is longer than another, add the difference in lengths towards the score.

To illustrate:
```python
letter_distance("house", "fly") = dist("h", "f") + dist("o", "l") + dist("u", "y") + dist(house.length, fly.length)

= |104 - 102| + |111 - 108| + |117 - 121| + |5 - 3|
= 2 + 3 + 4 + 2
= 11
```
## Examples
```python
letter_distance("sharp", "sharq") ➞ 1

letter_distance("abcde", "Abcde") ➞ 32

letter_distance("abcde", "bcdef") ➞ 5
```
## Notes

- Always start comparing the two strings from their first letter.
- Excess letters are not counted towards distance.
- Capital letters are included.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def letter_distance(str_a: str, str_b: str) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(letter_distance("house", "fly"), 11)

    def test_2(self):
        self.assertEqual(letter_distance("sharp", "sharq"), 1)

    def test_3(self):
        self.assertEqual(letter_distance("abcde", "bcdef"), 5)

    def test_4(self):
        self.assertEqual(letter_distance("abcde", "a"), 4)

    def test_5(self):
        self.assertEqual(letter_distance("abcde", "e"), 8)

    def test_6(self):
        self.assertEqual(letter_distance("abcde", "Abcde"), 32)

    def test_7(self):
        self.assertEqual(letter_distance("abcde", "A"), 36)

    def test_8(self):
        self.assertEqual(letter_distance("very", "fragile"), 67)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Letter Distance](https://edabit.com/challenge/XsqET8hSTBG2AR5kM)
