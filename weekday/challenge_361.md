# Challenge 361 - Reverse Words in a String

Given an input string, reverse the string word by word.

## Examples
```python
reverse_words("the sky is blue") ➞ "blue is sky the"

reverse_words("  hello world!  ") ➞ "world! hello"

reverse_words("a good   example") ➞ "example good a"
```
## Notes

- A word is defined as a sequence of non-space characters.
- The input string may contain leading or trailing spaces. However, your reversed string should not contain leading or trailing spaces.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def reverse_words(text: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(reverse_words("hello world!"), "world! hello")

    def test_2(self):
        self.assertEqual(reverse_words("blue is sky the"), "the sky is blue")

    def test_3(self):
        self.assertEqual(reverse_words("a good example"), "example good a")

    def test_4(self):
        self.assertEqual(
            reverse_words("fraud! of example another is this"),
            "this is another example of fraud!",
        )

    def test_5(self):
        self.assertEqual(reverse_words("man! the are You"), "You are the man!")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Reverse Words in a String](https://edabit.com/challenge/SfEretprfmbbcTChT)
