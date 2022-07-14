# Challenge 429 - White Spaces Between Lower and Uppercase Letters

Write a function that inserts a space between every instance of a lowercase character followed immediately by an uppercase character.

## Examples
```python
insert_whitespace("SheWalksToTheBeach") ➞ "She Walks To The Beach"

insert_whitespace("MarvinTalksTooMuch") ➞ "Marvin Talks Too Much"

insert_whitespace("TheGreatestUpsetInHistory") ➞ "The Greatest Upset In History"
```
## Notes

- Each word in the phrase will be at least two characters long.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def insert_whitespace(string: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(
            insert_whitespace("SheWalksToTheBeach"), "She Walks To The Beach"
        )

    def test_2(self):
        self.assertEqual(
            insert_whitespace("MarvinTalksTooMuch"), "Marvin Talks Too Much"
        )

    def test_3(self):
        self.assertEqual(
            insert_whitespace("HopelesslyDevotedToYou"), "Hopelessly Devoted To You"
        )

    def test_4(self):
        self.assertEqual(
            insert_whitespace("EvenTheBestFallDownSometimes"),
            "Even The Best Fall Down Sometimes",
        )

    def test_5(self):
        self.assertEqual(
            insert_whitespace("TheGreatestUpsetInHistory"),
            "The Greatest Upset In History",
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [White Spaces Between Lower and Uppercase Letters](https://edabit.com/challenge/TCbrjfMm2dPzQDbz5)
