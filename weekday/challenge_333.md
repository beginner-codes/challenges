# Challenge 333 - From A to Z

Given a string indicating a range of letters, create a function that returns a string that includes all the letters in that range, including the last letter. Note that if the range is given in capital letters, return the string in capitals also!

## Examples
```python
gimme_the_letters("a-z") ➞ "abcdefghijklmnopqrstuvwxyz"

gimme_the_letters("h-o") ➞ "hijklmno"

gimme_the_letters("Q-Z") ➞ "QRSTUVWXYZ"

gimme_the_letters("J-J") ➞ "J"
```
## Notes

- A hyphen will separate the two letters in the string.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def gimme_the_letters(letter_range: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(gimme_the_letters("a-z"), "abcdefghijklmnopqrstuvwxyz")

    def test_2(self):
        self.assertEqual(gimme_the_letters("h-o"), "hijklmno")

    def test_3(self):
        self.assertEqual(gimme_the_letters("Q-Z"), "QRSTUVWXYZ")

    def test_4(self):
        self.assertEqual(gimme_the_letters("J-J"), "J")

    def test_5(self):
        self.assertEqual(gimme_the_letters("a-b"), "ab")

    def test_6(self):
        self.assertEqual(gimme_the_letters("A-A"), "A")

    def test_7(self):
        self.assertEqual(gimme_the_letters("g-i"), "ghi")

    def test_8(self):
        self.assertEqual(gimme_the_letters("H-I"), "HI")

    def test_9(self):
        self.assertEqual(gimme_the_letters("y-z"), "yz")

    def test_10(self):
        self.assertEqual(gimme_the_letters("e-k"), "efghijk")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [From A to Z](https://edabit.com/challenge/Abo5qakEcntamMZ8p)
