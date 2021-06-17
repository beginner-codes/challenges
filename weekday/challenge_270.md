# Challenge 270 - Same on Both Ends

Given a sentence, return the number of words which have the same first and last letter.

## Examples
```python
countSameEnds("Pop! goes the balloon") ➞ 1

countSameEnds("And the crowd goes wild!") ➞ 0

countSameEnds("No I am not in a gang.") ➞ 1
```
## Notes

- Don't count single character words (such as `"I"` and `"A"`).
- The function should not be case-sensitive, meaning a capital `"P"` should match with a lowercase one.
- Mind the punctuation!

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def count_same_ends(sentence: str) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(count_same_ends("Pop! the balloon!"), 1)

    def test_2(self):
        self.assertEqual(count_same_ends("My mom is not a nun."), 2)

    def test_3(self):
        self.assertEqual(count_same_ends("A fine morning"), 0)

    def test_4(self):
        self.assertEqual(count_same_ends("And the crowd goes wild!"), 0)

    def test_5(self):
        self.assertEqual(count_same_ends("No I am not in a gang."), 1)

    def test_6(self):
        self.assertEqual(count_same_ends("Taste the difference"), 0)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Same on Both Ends](https://edabit.com/challenge/JDDeK9jSFKJbfzhMt)
