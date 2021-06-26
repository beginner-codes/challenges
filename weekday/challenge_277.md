# Challenge 277 - Distance to Nearest Vowel

Write a function that takes in a string and for each character, returns the distance to the nearest vowel in the string. If the character is a vowel itself, return `0`.

## Examples
```python
distance_to_nearest_vowel("aaaaa") ➞ [0, 0, 0, 0, 0]

distance_to_nearest_vowel("babbb") ➞ [1, 0, 1, 2, 3]

distance_to_nearest_vowel("abcdabcd") ➞ [0, 1, 2, 1, 0, 1, 2, 3]

distance_to_nearest_vowel("shopper") ➞ [2, 1, 0, 1, 1, 0, 1]
```
## Notes

- All input strings will contain at least one vowel.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def distance_to_nearest_vowel(string: str) -> list[int]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(distance_to_nearest_vowel("aaaaa"), [0, 0, 0, 0, 0])

    def test_2(self):
        self.assertListEqual(distance_to_nearest_vowel("bba"), [2, 1, 0])

    def test_3(self):
        self.assertListEqual(distance_to_nearest_vowel("abbb"), [0, 1, 2, 3])

    def test_4(self):
        self.assertListEqual(distance_to_nearest_vowel("abab"), [0, 1, 0, 1])

    def test_5(self):
        self.assertListEqual(distance_to_nearest_vowel("babbb"), [1, 0, 1, 2, 3])

    def test_6(self):
        self.assertListEqual(distance_to_nearest_vowel("baaab"), [1, 0, 0, 0, 1])

    def test_7(self):
        self.assertListEqual(
            distance_to_nearest_vowel("abcdabcd"), [0, 1, 2, 1, 0, 1, 2, 3]
        )

    def test_8(self):
        self.assertListEqual(
            distance_to_nearest_vowel("abbaaaaba"), [0, 1, 1, 0, 0, 0, 0, 1, 0]
        )

    def test_9(self):
        self.assertListEqual(
            distance_to_nearest_vowel("treesandflowers"),
            [2, 1, 0, 0, 1, 0, 1, 2, 2, 1, 0, 1, 0, 1, 2],
        )

    def test_10(self):
        self.assertListEqual(
            distance_to_nearest_vowel("pokerface"), [1, 0, 1, 0, 1, 1, 0, 1, 0]
        )

    def test_11(self):
        self.assertListEqual(
            distance_to_nearest_vowel("beautiful"), [1, 0, 0, 0, 1, 0, 1, 0, 1]
        )

    def test_12(self):
        self.assertListEqual(
            distance_to_nearest_vowel("rythmandblues"),
            [5, 4, 3, 2, 1, 0, 1, 2, 2, 1, 0, 0, 1],
        )

    def test_13(self):
        self.assertListEqual(
            distance_to_nearest_vowel("shopper"), [2, 1, 0, 1, 1, 0, 1]
        )

    def test_14(self):
        self.assertListEqual(
            distance_to_nearest_vowel("singingintherain"),
            [1, 0, 1, 1, 0, 1, 1, 0, 1, 2, 1, 0, 1, 0, 0, 1],
        )

    def test_15(self):
        self.assertListEqual(
            distance_to_nearest_vowel("sugarandspice"),
            [1, 0, 1, 0, 1, 0, 1, 2, 2, 1, 0, 1, 0],
        )

    def test_16(self):
        self.assertListEqual(
            distance_to_nearest_vowel("totally"), [1, 0, 1, 0, 1, 2, 3]
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Distance to Nearest Vowel](https://edabit.com/challenge/jWHkKc2pYmgobRL8R)
