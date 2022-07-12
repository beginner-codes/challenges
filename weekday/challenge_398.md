# Challenge 398 - Remove Repeated Characters

Create a function that will remove any repeated characters in the words passed to the function. Not just consecutive characters, but characters repeating anywhere in the input.

## Examples
```python
unrepeated("hello") ➞ "helo"

unrepeated("aaaaa") ➞ "a"

unrepeated("WWE!!!") ➞ "WE!"

unrepeated("call 911") ➞ "cal 91"
```
## Notes

- Input includes special characters and numbers.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def unrepeated(string: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(unrepeated("hello"), "helo")

    def test_2(self):
        self.assertEqual(unrepeated("aaaaa"), "a")

    def test_3(self):
        self.assertEqual(unrepeated("WWE!!!"), "WE!")

    def test_4(self):
        self.assertEqual(unrepeated("call 911"), "cal 91")

    def test_5(self):
        self.assertEqual(unrepeated("altwaff test"), "altwf es")

    def test_6(self):
        self.assertEqual(unrepeated("Mississippi"), "Misp")

    def test_7(self):
        self.assertEqual(unrepeated("Tennessee"), "Tens")

    def test_8(self):
        self.assertEqual(unrepeated("Massachusetts"), "Maschuet")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Remove Repeated Characters](https://edabit.com/challenge/5fjAbvQwW3akZDior)
