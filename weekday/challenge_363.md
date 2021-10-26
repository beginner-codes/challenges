# Challenge 363 - Find the Shared Letters between Two Strings

Given two strings, create a function that returns a string containing only the letters shared between the two.

## Examples
```python
shared_letters("house", "home") ➞ "eho"

shared_letters("Micky", "mouse") ➞ "m"

shared_letters("house", "villa") ➞ ""
```
## Notes

- If none of the letters are shared, return an empty string.
- The function should be case insensitive (e.g. comparing `A` and `a` should return `a`).
- Sort the resulting string alphabetically before returning it.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def shared_letters(word_a: str, word_b) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(shared_letters("house", "home"), "eho")

    def test_2(self):
        self.assertEqual(shared_letters("Micky", "mouse"), "m")

    def test_3(self):
        self.assertEqual(shared_letters("house", "villa"), "")

    def test_4(self):
        self.assertEqual(shared_letters("Aa", "aA"), "a")

    def test_5(self):
        self.assertEqual(
            shared_letters("https://www.example.com", "https://www.canada.ca"),
            "./:achpstw",
        )

    def test_6(self):
        self.assertEqual(shared_letters("BeginnerCodes", "Matt"), "")

    def test_7(self):
        self.assertEqual(shared_letters("Javascript", "Python"), "pt")

    def test_8(self):
        self.assertEqual(
            shared_letters("Functional programming", "Object oriented programming"),
            " acgimnoprt",
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Find the Shared Letters between Two Strings](https://edabit.com/challenge/XgJ3L3GF7o2dEaPAW)
