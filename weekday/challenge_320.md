# Challenge 320 - String Match by Two Letters

Create a function that takes two strings, `a` and `b`. Return the number of times the two strings contain the same two letters at the same index. The two letters must appear at consecutive indices.

For example, if `a = "bboiizz"` and `b = "bbuiiz"`, your function should return `3`, since the `"bb"`, `"ii"`, and `"iz"` appear at the same place in both strings.

## Examples
```python
str_match_by2char("yytaazz", "yyjaaz") ➞ 3

str_match_by2char("edabit", "ed") ➞ 1

str_match_by2char("", "") ➞ 0
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def count_two_character_matches(string_a: str, string_b: str) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(count_two_character_matches("jjcAAzz", "jjBAAz"), 3)

    def test_2(self):
        self.assertEqual(count_two_character_matches("ABcd", "ABcD"), 2)

    def test_3(self):
        self.assertEqual(count_two_character_matches("ABc", "Ajc"), 0)

    def test_4(self):
        self.assertEqual(count_two_character_matches("edabit", "ed"), 1)

    def test_5(self):
        self.assertEqual(count_two_character_matches("ed", "edabit"), 1)

    def test_6(self):
        self.assertEqual(count_two_character_matches("e", "edabit"), 0)

    def test_7(self):
        self.assertEqual(count_two_character_matches("", "edabit"), 0)

    def test_8(self):
        self.assertEqual(count_two_character_matches("AABBccDD", "ABBBjjD"), 1)

    def test_9(self):
        self.assertEqual(count_two_character_matches("AAjjAAjj", "iAjjAi"), 3)

    def test_10(self):
        self.assertEqual(count_two_character_matches("iAjjAi", "AAjjAAjj"), 3)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [String Match by Two Letters](https://edabit.com/challenge/qkBR9guzewqTztLPM)
