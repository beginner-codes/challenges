# Challenge 238 - Uppercase Counting

Create a function which counts all the uppercase letters in a list of words.

## Examples
```python
count_uppercase(["SOLO", "hello", "Tea", "wHat"]) ➞ 6

count_uppercase(["little", "lower", "down"]) ➞ 0

count_uppercase(["EDAbit", "Educate", "Coding"]) ➞ 5
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def count_uppercase(words: list[str]) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(count_uppercase(["SOLO", "hello", "Tea", "wHat"]), 6)

    def test_2(self):
        self.assertEqual(count_uppercase(["little", "lower", "down"]), 0)

    def test_3(self):
        self.assertEqual(count_uppercase(["BEGinner", "Dot", "Py"]), 5)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Adapted from Edabit: [Buggy Uppercase Counting](https://edabit.com/challenge/Hs7YDjZALCEPRPD6Z)
