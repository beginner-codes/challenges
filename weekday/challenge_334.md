# Challenge 334 - Extend the Vowels

Create a function that takes a word and extends all vowels by a number.

## Examples
```python
extend_vowels("Hello", 5) ➞ "Heeeeeelloooooo"

extend_vowels("Beginner.py", 3) ➞ "Beeeegiiiinneeeer.py"

extend_vowels("Extend", 0) ➞ "Extend"
```
## Notes

- Return `"invalid"` if num is not a positive integer.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def extend_vowels(word: str, extend: int) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(extend_vowels("Hello", 5), "Heeeeeelloooooo")

    def test_2(self):
        self.assertEqual(extend_vowels("Beginner.py", 3), "Beeeegiiiinneeeer.py")

    def test_3(self):
        self.assertEqual(extend_vowels("Extend", 0), "Extend")

    def test_4(self):
        self.assertEqual(extend_vowels("A", 10), "AAAAAAAAAAA")

    def test_5(self):
        self.assertEqual(extend_vowels("Z", 93), "Z")

    def test_6(self):
        self.assertEqual(extend_vowels("Vowel", 0.5), "invalid")

    def test_7(self):
        self.assertEqual(extend_vowels("Nice", -8), "invalid")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Extend the Vowels](https://edabit.com/challenge/nrrrYN8ZwhYjhvtS4)
