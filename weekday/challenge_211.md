# Challenge 211 - Layers in a Rug

Write a function that counts how many concentric layers are in the pattern on a rug.

## Examples
```python
count_layers([
  "AAAA",
  "ABBA",
  "AAAA"
]) ➞ 2

count_layers([
  "AAAAAAAAA",
  "ABBBBBBBA",
  "ABBAAABBA",
  "ABBBBBBBA",
  "AAAAAAAAA"
]) ➞ 3

count_layers([
  "AAAAAAAAAAA",
  "AABBBBBBBAA",
  "AABCCCCCBAA",
  "AABCAAACBAA",
  "AABCADACBAA",
  "AABCAAACBAA",
  "AABCCCCCBAA",
  "AABBBBBBBAA",
  "AAAAAAAAAAA"
]) ➞ 5
```
## Notes

- Multiple layers can share the same component so count them separately.
- Layers will be horizontally and vertically symmetric.
- There will be at least one layer for each rug.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def count_layers(rug: list[str]) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(count_layers(["AAA"]), 1)

    def test_2(self):
        self.assertEqual(count_layers(["AAAA", "AAAA", "AAAA"]), 1)

    def test_3(self):
        self.assertEqual(count_layers(["AAAA", "ABBA", "AAAA"]), 2)

    def test_4(self):
        self.assertEqual(
            count_layers(
                ["AAAAAAAAA", "ABBBBBBBA", "ABBBBBBBA", "ABBBBBBBA", "AAAAAAAAA"]
            ),
            2,
        )

    def test_5(self):
        self.assertEqual(
            count_layers(
                ["AAAAAAAAA", "ABBBBBBBA", "ABBAAABBA", "ABBBBBBBA", "AAAAAAAAA"]
            ),
            3,
        )

    def test_6(self):
        self.assertEqual(
            count_layers(
                ["AAAAAAAAA", "ABBBBBBBA", "ABCCCCCBA", "ABBBBBBBA", "AAAAAAAAA"]
            ),
            3,
        )

    def test_7(self):
        self.assertEqual(
            count_layers(
                [
                    "AAAAAAAAAAA",
                    "AABBBBBBBAA",
                    "AABCCCCCBAA",
                    "AABCAAACBAA",
                    "AABCADACBAA",
                    "AABCAAACBAA",
                    "AABCCCCCBAA",
                    "AABBBBBBBAA",
                    "AAAAAAAAAAA",
                ]
            ),
            5,
        )

    def test_8(self):
        self.assertEqual(
            count_layers(
                [
                    "AAAAAAAAAAA",
                    "AABBBBBBBAA",
                    "AABCCCCCBAA",
                    "AABCAAACBAA",
                    "AABCABACBAA",
                    "AABCAAACBAA",
                    "AABCCCCCBAA",
                    "AABBBBBBBAA",
                    "AAAAAAAAAAA",
                ]
            ),
            5,
        )

    def test_9(self):
        self.assertEqual(
            count_layers(
                [
                    "AAAAAAAAAAA",
                    "AABBBBBBBAA",
                    "AABCCCCCBAA",
                    "AABCDDDCBAA",
                    "AABCDDDCBAA",
                    "AABCDDDCBAA",
                    "AABCCCCCBAA",
                    "AABBBBBBBAA",
                    "AAAAAAAAAAA",
                ]
            ),
            4,
        )

    def test_10(self):
        self.assertEqual(
            count_layers(
                [
                    "FFFFFFFFFFFFFFFFFFFFFFFFF",
                    "FFFFFFFFFFFFFFFFFFFFFFFFF",
                    "FFFFGGGGGGGGGGGGGGGGGFFFF",
                    "FFFFGGGAAAAAAAAAAAGGGFFFF",
                    "FFFFGGGAABBBBBBBAAGGGFFFF",
                    "FFFFGGGAABCCCCCBAAGGGFFFF",
                    "FFFFGGGAABCDDDCBAAGGGFFFF",
                    "FFFFGGGAABCDDDCBAAGGGFFFF",
                    "FFFFGGGAABCDDDCBAAGGGFFFF",
                    "FFFFGGGAABCCCCCBAAGGGFFFF",
                    "FFFFGGGAABBBBBBBAAGGGFFFF",
                    "FFFFGGGAAAAAAAAAAAGGGFFFF",
                    "FFFFGGGGGGGGGGGGGGGGGFFFF",
                    "FFFFFFFFFFFFFFFFFFFFFFFFF",
                    "FFFFFFFFFFFFFFFFFFFFFFFFF",
                ]
            ),
            6,
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Layers in a Rug](https://edabit.com/challenge/LaBMjgbMjf5BajczX)
