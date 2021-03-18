# Challenge 206 - Censor Words from List

Create a function that takes a string and censors any word from a given list. The text removed must be replaced by the given character.

## Examples
```python
censor_string(
    "Today is a Wednesday!",
    ["Today", "a"],
    "-"
) ➞ "----- is - Wednesday!"

censor_string(
    "The cow jumped over the moon.",
    ["cow", "over"],
    "*"
) ➞ "The *** jumped **** the moon."

censor_string(
    "Why did the chicken cross the road?",
    ["Did", "chicken", "road"],
    "*"
) ➞ "Why *** the ******* cross the ****?"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def censor_string(phrase: str, consor_words: list[str], censor_character: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(
            censor_string("The cow jumped over the moon.", ["cow", "over"], "*"),
            "The *** jumped **** the moon.",
        )

    def test_2(self):
        self.assertEqual(
            censor_string(
                "Why do my cats keep eating grass?", ["Why", "keep", "eating"], "!"
            ),
            "!!! do my cats !!!! !!!!!! grass?",
        )

    def test_3(self):
        self.assertEqual(
            censor_string(
                "How do I stop myself from using python!?", ["do", "stop", "using"], "-"
            ),
            "How -- I ---- myself from ----- python!?",
        )

    def test_4(self):
        self.assertEqual(
            censor_string(
                "If statements are pretty fun to use.",
                ["statements", "pretty", "to"],
                "~~",
            ),
            "If ~~~~~~~~~~~~~~~~~~~~ are ~~~~~~~~~~~~ fun ~~~~ use.",
        )

    def test_5(self):
        self.assertEqual(
            censor_string(
                "I'm dyslexic, but that deos'tn matter!", ["that", "matter!"], "?"
            ),
            "I'm dyslexic, but ???? deos'tn ???????",
        )

    def test_6(self):
        self.assertEqual(
            censor_string(
                "I should be doing work but I am doing this instead.",
                ["should", "but", "this"],
                "*",
            ),
            "I ****** be doing work *** I am doing **** instead.",
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Censor Words from List](https://edabit.com/challenge/zJSF5EfPe69e9sJAc)
