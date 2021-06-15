# Challenge 268 - Hitting the Jackpot

Create a function that takes in a tuple (slot machine outcome) and returns `True` if all elements in the tuple are identical, and `False` otherwise. The tuple will contain 4 elements.

## Examples
```python
is_jackpot(("@", "@", "@", "@")) ➞ True

is_jackpot(("abc", "abc", "abc", "abc")) ➞ True

is_jackpot(("SS", "SS", "SS", "SS")) ➞ True

is_jackpot(("&&", "&", "&&&", "&&&&")) ➞ False

is_jackpot(("SS", "SS", "SS", "Ss")) ➞ False
```
## Notes

- The elements must be exactly identical for there to be a jackpot.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def is_jackpot(result: tuple[str, str, str, str]) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(is_jackpot(("@", "@", "@", "@")))

    def test_2(self):
        self.assertTrue(is_jackpot(("!", "!", "!", "!")))

    def test_3(self):
        self.assertTrue(is_jackpot(("abc", "abc", "abc", "abc")))

    def test_4(self):
        self.assertTrue(is_jackpot(("karaoke", "karaoke", "karaoke", "karaoke")))

    def test_5(self):
        self.assertTrue(is_jackpot(("SS", "SS", "SS", "SS")))

    def test_6(self):
        self.assertFalse(is_jackpot((":(", ":)", ":|", ":|")))

    def test_7(self):
        self.assertFalse(is_jackpot(("&&", "&", "&&&", "&&&&")))

    def test_8(self):
        self.assertFalse(is_jackpot(("hee", "heh", "heh", "heh")))

    def test_9(self):
        self.assertFalse(is_jackpot(("SS", "SS", "SS", "Ss")))

    def test_10(self):
        self.assertFalse(is_jackpot(("SS", "SS", "Ss", "Ss")))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Hitting the Jackpot](https://edabit.com/challenge/hxyvTffvdT4E238CY)
