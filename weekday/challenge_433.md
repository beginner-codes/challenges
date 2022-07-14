# Challenge 433 - Average Word Length

Create a function that takes in a sentence and returns the average length of each word in that sentence. Round your result to two decimal places.

## Examples
```python
average_word_length("A B C.") ➞ 1.00

average_word_length("What a gorgeous day.") ➞ 4.00

average_word_length("Dude, this is so awesome!") ➞ 3.80
```
## Notes

- Ignore punctuation when counting the length of a word.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def average_word_length(string: str) -> float:
    return 0.0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(average_word_length("A B C."), 1.00)

    def test_2(self):
        self.assertEqual(average_word_length("What a gorgeous day."), 4.00)

    def test_3(self):
        self.assertEqual(average_word_length("Dude, this is so awesome!"), 3.80)

    def test_4(self):
        self.assertEqual(average_word_length("Working on my tan right now."), 3.67)

    def test_5(self):
        self.assertEqual(
            average_word_length("Having a blast partying in Las Vegas."), 4.29
        )

    def test_6(self):
        self.assertEqual(
            average_word_length("Have you ever wondered what Saturn looks like?"), 4.75
        )

    def test_7(self):
        self.assertEqual(
            average_word_length(
                "I just planted a young oak tree, wonder how tall it will grow in a few years?"
            ),
            3.47,
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Average Word Length](https://edabit.com/challenge/HpJCBwggQMDLWTHsM)
