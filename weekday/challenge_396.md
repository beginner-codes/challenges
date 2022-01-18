# Challenge 396 - First N Vowels

Write a function that returns the first `n` vowels of a string.

## Examples
```python
first_n_vowels("sharpening skills", 3) ➞ "aei"

first_n_vowels("major league", 5) ➞ "aoeau"

first_n_vowels("hostess", 5) ➞ "invalid"
```
## Notes

- Return `"invalid"` if the `n` exceeds the number of vowels in a string.
- Vowels are: `a`, `e`, `i`, `o`, `u`

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def first_n_vowels(string: str, num_vowels: int) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(first_n_vowels("sharpening skills", 3), "aei")

    def test_2(self):
        self.assertEqual(first_n_vowels("major league", 5), "aoeau")

    def test_3(self):
        self.assertEqual(first_n_vowels("crabby patty", 2), "aa")

    def test_4(self):
        self.assertEqual(first_n_vowels("shrimp", 1), "i")

    def test_5(self):
        self.assertEqual(first_n_vowels("shrimpy", 2), "invalid")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [First N Vowels](https://edabit.com/challenge/H2EyqacEnijCozCWs)
