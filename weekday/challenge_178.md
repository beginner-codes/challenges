# Challenge 178 - Neutralisation

Given two strings comprised of `+` and `-`, return a new string which shows how the two strings interact in the following way:

- When positives and positives interact, they remain positive.
- When negatives and negatives interact, they remain negative.
- But when negatives and positives interact, they become neutral, and are shown as the number `0`.

## Worked Example
```python
neutralise("+-+", "+--") ➞ "+-0"
# Compare the first characters of each string, then the next in turn.
# "+" against a "+" returns another "+".
# "-" against a "-" returns another "-".
# "+" against a "-" returns "0".
# Return the string of characters.
```
## Examples
```python
neutralise("--++--", "++--++") ➞ "000000"

neutralise("-+-+-+", "-+-+-+") ➞ "-+-+-+"

neutralise("-++-", "-+-+") ➞ "-+00"
```
## Notes

- The two strings will be the same length.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```py
import unittest


def neutralise(series_a: str, series_b: str) -> str:
    return ""  # Put your code here!!!


class Test(unittest.TestCase):
    def test_1(self):
        self.assertEqual(neutralise("--++--", "++--++"), "000000")

    def test_2(self):
        self.assertEqual(neutralise("-+-+-+", "-+-+-+"), "-+-+-+")

    def test_3(self):
        self.assertEqual(neutralise("-++-", "-+-+"), "-+00")

    def test_4(self):
        self.assertEqual(neutralise("--++", "++++"), "00++")

    def test_5(self):
        self.assertEqual(neutralise("+++--+---", "++----++-"), "++0--000-")

    def test_6(self):
        self.assertEqual(neutralise("-----", "-----"), "-----")

    def test_7(self):
        self.assertEqual(neutralise("-+", "++"), "0+")

    def test_8(self):
        self.assertEqual(neutralise("--", "-+"), "-0")

    def test_9(self):
        self.assertEqual(neutralise("-++", "+--"), "000")

    def test_10(self):
        self.assertEqual(neutralise("++-++--++-", "-+++-++-++"), "0+0+0000+0")

    def test_11(self):
        self.assertEqual(neutralise("-++-+-++-", "+-++++---"), "00+0+000-")

    def test_12(self):
        self.assertEqual(neutralise("---++-+--", "-+++--++-"), "-00+0-+0-")

    def test_13(self):
        self.assertEqual(neutralise("+-----+++-", "--+-+-++--"), "0-0-0-++0-")

    def test_14(self):
        self.assertEqual(neutralise("+-----+-", "---++-++"), "0--00-+0")

    def test_15(self):
        self.assertEqual(neutralise("-+--+-+---", "-+--+-+-+-"), "-+--+-+-0-")

    def test_16(self):
        self.assertEqual(neutralise("+-+", "-++"), "00+")

    def test_17(self):
        self.assertEqual(neutralise("-++", "-+-"), "-+0")

    def test_18(self):
        self.assertEqual(neutralise("---+", "-+++"), "-00+")

    def test_19(self):
        self.assertEqual(neutralise("+--", "+--"), "+--")

    def test_20(self):
        self.assertEqual(neutralise("--+++-+-", "+++++---"), "00+++-0-")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Reversible Inclusive List Ranges](https://edabit.com/challenge/zW9JME7XNew4tgCCE)

