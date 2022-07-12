# Challenge 310 - Box Completely Filled?

Create a function that checks if the box is completely filled with the asterisk symbol `*`.

## Examples
```python
completely_filled([
  "#####",
  "#***#",
  "#***#",
  "#***#",
  "#####"
]) ➞ True

completely_filled([
  "#####",
  "#* *#",
  "#***#",
  "#***#",
  "#####"
]) ➞ False

completely_filled([
  "###",
  "#*#",
  "###"
]) ➞ True

completely_filled([
  "##",
  "##"
]) ➞ True
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def completely_filled(box: list[str]) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(completely_filled(["#"]))

    def test_2(self):
        self.assertFalse(
            completely_filled(["#####", "#* *#", "#***#", "#***#", "#####"])
        )

    def test_3(self):
        self.assertTrue(completely_filled(["##", "##"]))

    def test_4(self):
        self.assertFalse(
            completely_filled(
                ["######", "#* **#", "#****#", "#* **#", "#*** #", "######"]
            )
        )

    def test_5(self):
        self.assertTrue(completely_filled(["###", "#*#", "###"]))

    def test_6(self):
        self.assertFalse(
            completely_filled(
                ["######", "#* **#", "#* **#", "#* **#", "#* **#", "######"]
            )
        )

    def test_7(self):
        self.assertTrue(
            completely_filled(
                ["######", "#****#", "#****#", "#****#", "#****#", "######"]
            )
        )

    def test_8(self):
        self.assertTrue(
            completely_filled(["#####", "#***#", "#***#", "#***#", "#####"])
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [All About Lambda Expressions: Adding Suffixes](https://edabit.com/challenge/nn7JKRBfq8iDcX8ZB)
