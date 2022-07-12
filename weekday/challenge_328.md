# Challenge 328 - Censor Words Longer Than Four Characters

Create a function that takes a string and censors words over four characters with `*`.

## Examples
```python
censor("The code is fourty") ➞ "The code is ******"

censor("Two plus three is five") ➞ "Two plus ***** is five"

censor("aaaa aaaaa 1234 12345") ➞ "aaaa ***** 1234 *****"
```
## Notes

- Don't censor words with exactly four characters.
- If all words have four characters or less, return the original string.
- The amount of `*` is the same as the length of the word.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def censor(string: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(censor("The code is fourty"), "The code is ******")

    def test_2(self):
        self.assertEqual(censor("Two plus three is five"), "Two plus ***** is five")

    def test_3(self):
        self.assertEqual(censor("aaaa aaaaa 1234 12345"), "aaaa ***** 1234 *****")

    def test_4(self):
        self.assertEqual(censor("abcdefghijklmnop"), "****************")

    def test_5(self):
        self.assertEqual(censor("a"), "a")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Censor Words Longer Than Four Characters](https://edabit.com/challenge/jWk79SoDXnfm8ymhw)
