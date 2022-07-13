# Challenge 343 - Club Entry

A night club will give you a word. For entrance, you need to provide the right number according to the provided word.

Every given word will have a doubled letter, like `"dd"` in "addition". To compute the correct number you need to find the doubled letter's position in the alphabet and multiply that number by 4.

Create a function that takes a word and returns the correct number.

## Examples
```python
club_entry("hill") ➞ 48
# 'l' is 12th letter in the alphabet
# 12*4 = 48

club_entry("apple") ➞ 64

club_entry("bee") ➞ 20
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def club_entry(word: str) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(club_entry("lettuce"), 80)

    def test_2(self):
        self.assertEqual(club_entry("hill"), 48)

    def test_3(self):
        self.assertEqual(club_entry("apple"), 64)

    def test_4(self):
        self.assertEqual(club_entry("addiction"), 16)

    def test_5(self):
        self.assertEqual(club_entry("bee"), 20)

    def test_6(self):
        self.assertEqual(club_entry("zz"), 104)

    def test_7(self):
        self.assertEqual(club_entry("mubashirr"), 72)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Club Entry](https://edabit.com/challenge/tK44PSWFuFzthwNJj)
