# Challenge 432 - Finish the Sentence You're On!

_POV: You are in an exam and time has just run out. While the teacher's back is turned, you hastily take the opportunity to finish scribbling down the last few words of the conclusion._

For this challenge, it takes `0.5` seconds to write a character (not including spaces). Given the full sentence and the unfinished sentence as inputs, return the time it takes to finish writing in seconds.

## Worked Example
```python
time_to_finish(
  "And so brings my conclusion to its conclusion.",
  "And so brings my conclusion to"
) ➞ 7

# "its" has 3 characters
# "conclusion." has 11 characters, including punctuation.
# 11 + 3 = 14
# 14 x 0.5 = 7
# Remember not to include spaces.
```
## Examples
```python
time_to_finish(
  "And so brings my conclusion to its conclusion.",
  "And so brings my conclusion to its conclus"
) ➞ 2

time_to_finish(
  "As a result, my point is still valid.",
  "As a result, my"
) ➞ 9

time_to_finish(
  "Thank you for reading my essay.",
  "T"
) ➞ 12.5
```
## Notes

- The unfinished sentence is always found at the start of a complete sentence.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def time_to_finish(sentence: str, unfinished: str) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(
            time_to_finish(
                "And so brings my conclusion to its conclusion.",
                "And so brings my conclusion to its conclus",
            ),
            2,
        )

    def test_2(self):
        self.assertEqual(
            time_to_finish("As a result, my point is still valid.", "As a result, my"),
            9,
        )

    def test_3(self):
        self.assertEqual(time_to_finish("Thank you for reading my essay.", "T"), 12.5)

    def test_4(self):
        self.assertEqual(
            time_to_finish(
                "Therefore, there was over there their only answer.",
                "Therefore, there w",
            ),
            13.5,
        )

    def test_5(self):
        self.assertEqual(
            time_to_finish(
                "And there, I end this thesis with a rock solid conclusion.",
                "And there, I end this thesis with a rock solid conclusion.",
            ),
            0,
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Finish the Sentence You're On!!](https://edabit.com/challenge/CXtsRKiRyAcGe2iEj)
