# Challenge 423 - Casino Security

You're head of security at a casino that has money being stolen from it. You get the data in the form of strings and you have to set off an alarm if a thief is detected.

- If there is no guard between thief and money, return `"ALARM!"`
- If the money is protected, return `"Safe"`

String Components:
- `x` Empty Space
- `T` Thief
- `G` Guard
- `$` Money

## Examples
```python
security("xxxxTTxGxx$xxTxxx") ➞ "ALARM!"

security("xxTxxG$xxxx$xxxx") ➞ "Safe"

security("TTxxxx$xxGxx$Gxxx") ➞ "ALARM!"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def security(string: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(security("xxTxxx$xxxTxxxGxxT"), "ALARM!")

    def test_2(self):
        self.assertEqual(security("xGxx$xxGxxxTTT"), "Safe")

    def test_3(self):
        self.assertEqual(security("TxGxx$xxx$xxxGxxT"), "Safe")

    def test_4(self):
        self.assertEqual(security("GxxxTxxGxxTxx$xx$xxTxxG"), "ALARM!")

    def test_5(self):
        self.assertEqual(security("xxGTxx$xx$xxxxxxG"), "ALARM!")

    def test_6(self):
        self.assertEqual(security("xxTxxxxxxxx$xGxxxxxxT"), "ALARM!")

    def test_7(self):
        self.assertEqual(security("xx$xxGxxxx$xxxxxxxxxxT"), "ALARM!")

    def test_8(self):
        self.assertEqual(security("xxxTxxxxT"), "Safe")

    def test_9(self):
        self.assertEqual(security("xxGxxxGGG"), "Safe")

    def test_10(self):
        self.assertEqual(security("x$xx$x$x$xx"), "Safe")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Casino Security](https://edabit.com/challenge/2jcxK7gpn6Z474kjz)
