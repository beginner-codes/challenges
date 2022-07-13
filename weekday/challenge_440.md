# Challenge 440 - Vowel Families

Write a function that selects all words that have all the same vowels (in any order and/or number) as the first word, including the first word.

## Examples
```python
same_vowel_group(["toe", "ocelot", "maniac"]) ➞ ["toe", "ocelot"]

same_vowel_group(["many", "carriage", "emit", "apricot", "animal"]) ➞ ["many"]

same_vowel_group(["hoops", "chuff", "bot", "bottom"]) ➞ ["hoops", "bot", "bottom"]
```
## Notes

- Words will contain only lowercase letters, and may contain whitespaces.
- Frequency does not matter (e.g. if the first word is "loopy", then you can include words with any number of o's, so long as they only contain o's, and not any other vowels).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def same_vowel_group(words: list[str]) -> list[str]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(
            same_vowel_group(["hoops", "chuff", "bot", "bottom"]),
            ["hoops", "bot", "bottom"],
        )

    def test_2(self):
        self.assertListEqual(
            same_vowel_group(["crop", "nomnom", "bolo", "yodeller"]),
            ["crop", "nomnom", "bolo"],
        )

    def test_3(self):
        self.assertListEqual(
            same_vowel_group(["semantic", "aimless", "beautiful", "meatless icecream"]),
            ["semantic", "aimless", "meatless icecream"],
        )

    def test_4(self):
        self.assertListEqual(
            same_vowel_group(["many", "carriage", "emit", "apricot", "animal"]),
            ["many"],
        )

    def test_5(self):
        self.assertListEqual(
            same_vowel_group(["toe", "ocelot", "maniac"]), ["toe", "ocelot"]
        )

    def test_6(self):
        self.assertListEqual(
            same_vowel_group(["a", "apple", "flat", "map", "shark"]),
            ["a", "flat", "map", "shark"],
        )

    def test_7(self):
        self.assertListEqual(
            same_vowel_group(["a", "aa", "ab", "abc", "aaac", "abe"]),
            ["a", "aa", "ab", "abc", "aaac"],
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Vowel Families](https://edabit.com/challenge/uwFHSRewNpmBNvbME)
