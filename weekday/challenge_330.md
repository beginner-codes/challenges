# Challenge 330 - Double Character Swap

Write a function to replace all instances of a character with another character and vice versa.

## Examples
```python
double_swap("aabbccc", "a", "b") ➞ "bbaaccc"

double_swap("random w#rds writt&n h&r&", "#", "&")
➞ "random w&rds writt#n h#r#"

double_swap("128 895 556 788 999", "8", "9")
➞ "129 985 556 799 888"
```
## Notes

- Both characters will show up at least once in the string.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def double_swap(string: str, character_1: str, character_2: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(double_swap("aabbccc", "a", "b"), "bbaaccc")

    def test_2(self):
        self.assertEqual(double_swap("random w#rds writt&n h&r&", "#", "&"), "random w&rds writt#n h#r#")

    def test_3(self):
        self.assertEqual(double_swap("128 895 556 788 999", "8", "9"), "129 985 556 799 888")

    def test_4(self):
        self.assertEqual(double_swap("mamma mia", "m", "a"), "amaam aim")

    def test_5(self):
        self.assertEqual(double_swap("**##**", "*", "#"), "##**##")

    def test_6(self):
        self.assertEqual(double_swap("123456789", "4", "5"), "123546789")

    def test_7(self):
        self.assertEqual(double_swap("445566&&", "4", "&"), "&&556644")

    def test_8(self):
        self.assertEqual(double_swap("!?@,.", ",", "."), "!?@.,")

    def test_9(self):
        self.assertEqual(double_swap("Q_Q T_T =.= >.<", "Q", "T"), "T_T Q_Q =.= >.<")

    def test_10(self):
        self.assertEqual(double_swap("(Q_Q) (T_T) (=.=) (>.<)", ")", "("), ")Q_Q( )T_T( )=.=( )>.<(")

    def test_11(self):
        self.assertEqual(double_swap("<>", ">", "<"), "><")

    def test_12(self):
        self.assertEqual(double_swap("001101", "1", "0"), "110010")

    def test_13(self):
        self.assertEqual(double_swap("!\"#$%&'()*+,-./0123456789:;<=>?@ABCDEFGHIJKLMNOPQRSTUVWXYZ[\]^_`abcdefghijklmnopqrstuvwxyz{|}~", "a", "b"), "!\"#$%&'()*+,-./0123456789:;<=>?@ABCDEFGHIJKLMNOPQRSTUVWXYZ[\]^_`bacdefghijklmnopqrstuvwxyz{|}~")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Double Character Swap](https://edabit.com/challenge/mHRyhyazjCoze5jSL)
