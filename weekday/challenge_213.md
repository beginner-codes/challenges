# Challenge 213 - Words With Duplicate Letters

Given a common phrase, return `False` if any individual word in the phrase contains duplicate letters. Return `True` otherwise.

## Examples
```python
no_duplicate_letters("Fortune favours the bold.") ➞ True

no_duplicate_letters("You can lead a horse to water, but you can't make him drink.") ➞ True

no_duplicate_letters("Look before you leap.") ➞ False
# Duplicate letters in "Look" and "before".

no_duplicate_letters("An apple a day keeps the doctor away.") ➞ False
# Duplicate letters in "apple", "keeps", "doctor", and "away".
```
## Notes

- Letter matches are case-insensitive.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def no_duplicate_letters(phrase: str) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(no_duplicate_letters("Easy does it."))

    def test_2(self):
        self.assertFalse(no_duplicate_letters("So far, so good."))

    def test_3(self):
        self.assertFalse(no_duplicate_letters("Better late than never."))

    def test_4(self):
        self.assertTrue(no_duplicate_letters("Beat around the bush."))

    def test_5(self):
        self.assertFalse(no_duplicate_letters("Give them the benefit of the doubt."))

    def test_6(self):
        self.assertFalse(no_duplicate_letters("Your guess is as good as mine."))

    def test_7(self):
        self.assertTrue(no_duplicate_letters("Make a long story short."))

    def test_8(self):
        self.assertTrue(no_duplicate_letters("Go back to the drawing board."))

    def test_9(self):
        self.assertTrue(no_duplicate_letters("Wrap your head around something."))

    def test_10(self):
        self.assertFalse(no_duplicate_letters("Get your act together."))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Maze Escape](https://edabit.com/challenge/tbz5ji3ocwzAeLQNa)
