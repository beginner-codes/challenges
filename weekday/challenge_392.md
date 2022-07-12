# Challenge 392 - Percentage of Box Filled In

Create a function that calculates what percentage of the box is filled in. Give your answer as a string percentage rounded to the nearest integer.

## Examples
```python
percent_filled([
  "####",
  "#  #",
  "#o #",
  "####"
]) ➞ "25%"

# One element out of four spaces.

percent_filled([
  "#######",
  "#o oo #",
  "#######"
]) ➞ "60%"

# Three elements out of five spaces.

percent_filled([
  "######",
  "#ooo #",
  "#oo  #",
  "#    #",
  "#    #",
  "######"
]) ➞ "31%"

# Five elements out of sixteen spaces.
```
## Notes

- Only `"o"` will fill the box and also `"o"` will not be found outside the box.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def percent_filled(box: list[str]) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(percent_filled(["####", "#  #", "#o #", "####"]), "25%")

    def test_2(self):
        self.assertEqual(percent_filled(["#######", "#o oo #", "#######"]), "60%")

    def test_3(self):
        self.assertEqual(
            percent_filled(
                ["######", "#ooo #", "#oo  #", "#    #", "#    #", "######"]
            ),
            "31%",
        )

    def test_4(self):
        self.assertEqual(percent_filled(["####", "#  #", "####"]), "0%")

    def test_5(self):
        self.assertEqual(percent_filled(["###", "#o#", "###"]), "100%")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Percentage of Box Filled In](https://edabit.com/challenge/ENJTPoWCyEGgnXYjM)
