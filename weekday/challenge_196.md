# Challenge 196 - Change Every Letter to the Next Letter

Write a function that changes every letter to the next letter of the alphabet:
```python
"a" becomes "b"
"b" becomes "c"
"d" becomes "e"
and so on ...
```
## Examples
```python
move("hello") ➞ "ifmmp"

move("bye") ➞ "czf"

move("welcome") ➞ "xfmdpnf"
```
## Notes

- Z's will wrap around to become A's

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def move(word: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(move("hello"), "ifmmp")

    def test_2(self):
        self.assertEqual(move("lol"), "mpm")

    def test_3(self):
        self.assertEqual(move("bye"), "czf")

    def test_4(self):
        self.assertEqual(move("zebra"), "afcsb")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Change Every Letter to the Next Letter](https://edabit.com/challenge/oiHH7qocTyM3JqNf8)
