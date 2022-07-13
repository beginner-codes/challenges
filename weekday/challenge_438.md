# Challenge 438 - A Subtle Switcheroo

Create a function which replaces all instances of `"nts"` with `"nce"` and vice versa if they are at the end of a word.

## Examples
```
switcheroo("The elephants in France were chased by ants!") ➞ "The elephance in Frants were chased by ance!"

switcheroo("While he rants, I fall into a trance...") ➞ "While he rance, I fall into a trants..."

switcheroo("Bounced over the fence!") ➞ "Bounced over the fents!"
```
## Notes

- Empty strings should return just an empty string (see the second example).
- Ignore punctuation and any instances where `"nts"` or `"nce"` are not at the end of a word (see the third example).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def switcheroo(string: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(
            switcheroo("While he rants, I fall into a trance..."),
            "While he rance, I fall into a trants...",
        )

    def test_2(self):
        self.assertEqual(
            switcheroo("The elephants in France were chased by ants!"),
            "The elephance in Frants were chased by ance!",
        )

    def test_3(self):
        self.assertEqual(
            switcheroo("Bounced over the fence!"), "Bounced over the fents!"
        )

    def test_4(self):
        self.assertEqual(switcheroo("Face"), "Face", "Replace nce, not just ce")

    def test_5(self):
        self.assertEqual(switcheroo("Fats"), "Fats", "Replace nts, not just ts")

    def test_6(self):
        self.assertEqual(switcheroo(""), "")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [A Subtle Switcheroo](https://edabit.com/challenge/o7u9hqTW5AY3SoZgT)
