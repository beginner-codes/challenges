# Challenge 413 - Switching Between Pencils

When coloring a striped pattern, you may start by coloring each square sequentially, meaning you spend time needing to switch coloring pencils.

Create a function where given a list of colors, return how long it takes to color the whole pattern. Note the following times:

- It takes 1 second to switch between pencils.
- It takes 2 seconds to color a square.

See the example below for clarification.
```python
color_pattern_times(["Red", "Blue", "Red", "Blue", "Red"]) ➞ 14

# There are 5 colors so it takes 2 seconds to color each one (2 x 5 = 10).
# You need to switch the pencils 4 times and it takes 1 second to switch (1 x 4 = 4).
# 10 + 4 = 14
```
## Examples
```python
color_pattern_times(["Blue"]) ➞ 2

color_pattern_times(["Red", "Yellow", "Green", "Blue"]) ➞ 11

color_pattern_times(["Blue", "Blue", "Blue", "Red", "Red", "Red"]) ➞ 13
```
## Notes

- Only change coloring pencils if the next color is different to the color before it.
- Return a number in seconds.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def color_pattern_times(colors: list[str]) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(
            color_pattern_times(
                ["Red", "Green", "Blue", "Yellow", "Red", "Red",
                 "Yellow", "Green", "Green", "Green", "Red", "Blue",
                 "Yellow", "Blue", "Green", "Green", "Red", "Red",
                 "Red", "Blue", "Green", "Red", "Blue", "Blue", "Red",
                 "Blue"]
            ),
            70,
        )

    def test_2(self):
        self.assertEqual(
            color_pattern_times(
                ["Red", "Blue", "Yellow", "Blue", "Green", "Green",
                 "Yellow", "Green", "Blue", "Blue", "Blue", "Red",
                 "Blue", "Red", "Green", "Red"]
            ),
            44,
        )

    def test_3(self):
        self.assertEqual(color_pattern_times(["Yellow", "Green", "Blue"]), 8)

    def test_4(self):
        self.assertEqual(
            color_pattern_times(
                ["Green", "Green", "Red", "Green", "Yellow", "Red",
                 "Red", "Green", "Red", "Green"]
            ),
            27,
        )

    def test_5(self):
        self.assertEqual(color_pattern_times(["Red"]), 2)

if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Switching Between Pencils](https://edabit.com/challenge/MFteyMABeuGaga3a7)
