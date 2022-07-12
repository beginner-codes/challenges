# Challenge 355 - Abbreviating a Sentence

Create a function which takes a sentence and returns its abbreviation. Get all of the words over or equal to `n` characters in length and return the first letter of each, capitalised and overall returned as a single string.

## Examples
```python
abbreviate("do it yourself") ➞ "Y"

abbreviate("do it yourself", 2) ➞ "DIY"
# "do" and "it" are included because the second parameter specified that word lengths 2 are allowed.

abbreviate("attention AND deficit OR hyperactivity THE disorder") ➞ "ADHD"
# Words below the default 4 characters are not included in the abbreviation.

abbreviate("the acronym of long word lengths", 5) ➞ "AL"
# "acronym" and "lengths" have 5 or more characters.
```
## Notes

- There may not be an argument given for `n` so set the default to `4`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def abbreviate(phrase: str, min_length: int = 4) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(abbreviate("do it yourself", 2), "DIY")

    def test_2(self):
        self.assertEqual(
            abbreviate("attention AND deficit OR hyperactivity THE disorder"), "ADHD"
        )

    def test_3(self):
        self.assertEqual(abbreviate("the acronym of long word lengths", 5), "AL")

    def test_4(self):
        self.assertEqual(abbreviate("laugh out loud"), "LL")

    def test_5(self):
        self.assertEqual(abbreviate("Keep It Simple Stupid"), "KSS")

    def test_6(self):
        self.assertEqual(abbreviate("laugh out loud", 3), "LOL")

    def test_7(self):
        self.assertEqual(abbreviate("Keep It Simple Stupid", 2), "KISS")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Abbreviating a Sentence](https://edabit.com/challenge/QWAqDyd9RXqyrNyo3)
