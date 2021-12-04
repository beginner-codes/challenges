# Challenge 383 - Reverse Sort: Lexical and Length

Write a function that sorts the words in a given string lexicographically (lexical sort) and by length in reverse order.

## Examples
```python
reverse_sort("You've rocked the pragmatic world in the making!") 
 ➞ "pragmatic making! You've rocked world the the in"

reverse_sort("Tesh makes my world worth enjoying and living for.")
 ➞ "enjoying living worth world makes Tesh for. and my"

reverse_sort(reverseSort("Shaken by the bloody truth and crazy lies.")
 ➞ "Shaken bloody truth lies. crazy the and by"

reverse_sort("Programming in Python is a lot of fun.")
 ➞ "Programming Python fun. lot of is in a"
```
## Notes
- Special characters, punctuations and symbols are part of the word that directly precede it.
- The space character separates each word in the given string.
- Case insensitive sorting is required.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def reverse_sort(string: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(
            reverse_sort("You've rocked the pragmatic world in the making!"),
            "pragmatic making! You've rocked world the the in",
        )

    def test_2(self):
        self.assertEqual(
            reverse_sort("Tesh makes my world worth enjoying and living for."),
            "enjoying living worth world makes Tesh for. and my",
        )

    def test_3(self):
        self.assertEqual(
            reverse_sort("Shaken by the bloody truth and crazy lies."),
            "Shaken bloody truth lies. crazy the and by",
        )

    def test_4(self):
        self.assertEqual(
            reverse_sort("Java streams and collections are fun to program with!"),
            "collections streams program with! Java fun are and to",
        )

    def test_5(self):
        self.assertEqual(
            reverse_sort("Tesha is a woman of true substance and a beauty."),
            "substance beauty. woman Tesha true and of is a a",
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Reverse Sort: Lexical and Length](https://edabit.com/challenge/pEG8G4se5WBQkckF2)
