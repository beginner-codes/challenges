# Challenge 264 - Count the Letters and Digits

Write a function that takes a string and calculates the number of letters and digits in it. Return the result in a dictionary.

## Examples
```python
count_all("Hello World") ➞ { "LETTERS":  10, "DIGITS": 0 }

count_all("H3ll0 Wor1d") ➞ { "LETTERS":  7, "DIGITS": 3 }

count_all("149990") ➞ { "LETTERS": 0, "DIGITS": 6 }
```
## Notes

- Spaces are not letters (does that even need to be said? lol).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def count_all(string: str) -> dict[str, int]:
    return {}  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(count_all("Hello"), {"LETTERS": 5, "DIGITS": 0})

    def test_2(self):
        self.assertEqual(count_all("137"), {"LETTERS": 0, "DIGITS": 3})

    def test_3(self):
        self.assertEqual(count_all("H3LL0"), {"LETTERS": 3, "DIGITS": 2})

    def test_4(self):
        self.assertEqual(count_all("149990"), {"LETTERS": 0, "DIGITS": 6})

    def test_5(self):
        self.assertEqual(
            count_all("Beginner.py 2021"),
            {"LETTERS": 10, "DIGITS": 4},
        )

    def test_6(self):
        self.assertEqual(count_all("    "), {"LETTERS": 0, "DIGITS": 0})


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Count the Letters and Digits](https://edabit.com/challenge/KEz3TAQfh9WxSZMLH)
