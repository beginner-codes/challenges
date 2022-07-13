# Challenge 348 - Longest Word

Write a function that finds the longest word in a sentence. If two or more words are found, return the first longest word. Characters such as apostrophe, comma, period (and the like) count as part of the word (e.g. O'Connor is 8 characters long).

## Examples
```python
longest_word("Margaret's toy is a pretty doll.") ➞ "Margaret's"

longest_word("A thing of beauty is a joy forever.") ➞ "forever."
  
longest_word("Forgetfulness is by all means powerless!") ➞ "Forgetfulness"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def longest_word(sentence: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(longest_word("Hello darkness my old friend."), "darkness")

    def test_2(self):
        self.assertEqual(longest_word("Hello there mate."), "Hello")

    def test_3(self):
        self.assertEqual(longest_word("Margaret's toy is a pretty doll."), "Margaret's")

    def test_4(self):
        self.assertEqual(longest_word("A thing of beauty is a joy forever."), "forever.")

    def test_5(self):
        self.assertEqual(longest_word("Forgetfulness is by all means powerless!"), "Forgetfulness")

    def test_6(self):
        self.assertEqual(
            longest_word("The word 'strengths' is the longest and most commonly used word with a single vowel."),
            "'strengths'",
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Reversing a Binary String](https://edabit.com/challenge/WPojigJER35bJT6YH)
