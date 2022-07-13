# Challenge 409 - Divide a Fraction by Two

Create a function that takes a fraction as an argument and returns half of it.

## Examples
```python
half_a_fraction("1/2") ➞ "1/4"

half_a_fraction("6/8") ➞ "3/8"

half_a_fraction("3/8") ➞ "3/16"
```
## Notes

- Always return the simplified fraction.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def half_a_fraction(fraction: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(half_a_fraction("1/2"), "1/4")

    def test_2(self):
        self.assertEqual(half_a_fraction("2/3"), "1/3")

    def test_3(self):
        self.assertEqual(half_a_fraction("3/8"), "3/16")

    def test_4(self):
        self.assertEqual(half_a_fraction("39/46"), "39/92")

    def test_5(self):
        self.assertEqual(half_a_fraction("52/97"), "26/97")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Divide a Fraction by Two](https://edabit.com/challenge/egHeSWSjHTgzMysBX)
