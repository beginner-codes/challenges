# Challenge 442 - Extending The String

Make two functions:

- `consonants(word)` which returns the number of consonants in a word when called.
- `vowels(word)` which returns the number of vowels in a word when called.

## Examples
```python
vowels('Jameel SAEB') ➞ 5

consonants('He|\o mY Fr*end') ➞ 7

consonants("Smithsonian") ➞ 7
vowels("Smithsonian") ➞ 4
```
## Notes
- Vowels are: `a`, `e`, `i`, `o`, `u`.
- Spaces and special characters count neither as consonants nor as vowels.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def consonants(string: str) -> int:
    return 0  # Put your code here!!!


def vowels(string: str) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(vowels("Jameel SAEB"), 5)

    def test_2(self):
        self.assertEqual(consonants("Jameel SAEB"), 5)

    def test_3(self):
        self.assertEqual(consonants("Peter PANS"), 6)

    def test_4(self):
        self.assertEqual(vowels("Peter PAN"), 3)

    def test_5(self):
        self.assertEqual(consonants("hello"), 3)

    def test_6(self):
        self.assertEqual(vowels("hello"), 2)

    def test_7(self):
        self.assertEqual(consonants("grEatly"), 5)

    def test_8(self):
        self.assertEqual(vowels("greatly"), 2)

    def test_9(self):
        self.assertEqual(vowels("He|\o mY Fr*end"), 3)

    def test_10(self):
        self.assertEqual(consonants("He|\o mY Fr*end"), 7)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Extending The String](https://edabit.com/challenge/zxAXEgpjQ3XrLs2K7)
