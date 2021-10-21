# Challenge 360 - Letters Only

Write a function that checks if a given string consists of only letters and spaces and that every letter is lower case.

## Examples
```python
letters_only("PYTHON") ➞ False

letters_only("python") ➞ True

letters_only("12321313") ➞ False

letters_only("i have spaces") ➞ True

letters_only("i have numbers(1-10)") ➞ False

letters_only("") ➞ False
```
## Notes

- Empty arguments will always return `False`.
- Input values will be mixed (symbols, letters, numbers).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def letters_only(text: str) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertFalse(letters_only("PYTHON"))

    def test_2(self):
        self.assertTrue(letters_only("python"))

    def test_3(self):
        self.assertTrue(letters_only("html css javascript"))

    def test_4(self):
        self.assertFalse(letters_only("12321313"))

    def test_5(self):
        self.assertFalse(letters_only("@-=001-302;4'23"))

    def test_6(self):
        self.assertTrue(letters_only("the quick brown fox"))

    def test_7(self):
        self.assertFalse(letters_only("hello 123 world"))

    def test_8(self):
        self.assertTrue(letters_only("i have spaces"))

    def test_9(self):
        self.assertFalse(letters_only(""))

    def test_10(self):
        self.assertFalse(letters_only("i have numbers 1 and 2)"))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Letters Only](https://edabit.com/challenge/aSZ28TjivazB3aErL)
