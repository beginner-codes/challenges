# Challenge 399 - Broken Keyboard

Given what is supposed to be typed and what is actually typed, write a function that returns the broken keys.

## Examples
```python
find_broken_keys("happy birthday", "hawwy birthday") ➞ ["p"]

find_broken_keys("starry night", "starrq light") ➞ ["y", "n"]

find_broken_keys("beethoven", "affthoif5") ➞ ["b", "e", "v", "n"]
```
## Notes

- Broken keys should be ordered by when they first appear in the sentence.
- Only one broken key per letter should be listed.
- Letters will all be in lower case.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def find_broken_keys(expected: str, actual: str) -> list[str]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(
            find_broken_keys("happy birthday", "hawwy birthday"), ["p"]
        )

    def test_2(self):
        self.assertListEqual(
            find_broken_keys("starry night", "starrq light"), ["y", "n"]
        )

    def test_3(self):
        self.assertListEqual(
            find_broken_keys("beethoven", "affthoif5"), ["b", "e", "v", "n"]
        )

    def test_4(self):
        self.assertListEqual(
            find_broken_keys("mozart", "aiwgvx"), ["m", "o", "z", "a", "r", "t"]
        )

    def test_5(self):
        self.assertListEqual(find_broken_keys("5678", "4678"), ["5"])

    def test_6(self):
        self.assertListEqual(find_broken_keys("!!??$$", "$$!!??"), ["!", "?", "$"])


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Broken Keyboard](https://edabit.com/challenge/J2apiSnJE4RaGTj6x)
