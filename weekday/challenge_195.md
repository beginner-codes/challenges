# Challenge 195 - Letters Shared Between Two Words

Create a function that returns the number of characters shared between two words.

## Examples
```python
shared_letters("apple", "meaty") ➞ 2
# Since "ea" is shared between "apple" and "meaty".

shared_letters("fan", "forsook") ➞ 1

shared_letters("spout", "shout") ➞ 4
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def shared_letters(word_a: str, word_b: str) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(shared_letters("apple", "meaty"), 2)

    def test_2(self):
        self.assertEqual(shared_letters("fan", "forsook"), 1)

    def test_3(self):
        self.assertEqual(shared_letters("spout", "shout"), 4)

    def test_4(self):
        self.assertEqual(shared_letters("took", "taken"), 2)

    def test_5(self):
        self.assertEqual(shared_letters("mentor", "terminal"), 5)

    def test_6(self):
        self.assertEqual(shared_letters("class", "last"), 3)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on /r/dailyprogrammer: [\[2018-04-23\] Challenge #358 \[Easy\] Decipher The Seven Segments](https://www.reddit.com/r/dailyprogrammer/comments/8eger3/20180423_challenge_358_easy_decipher_the_seven/)
