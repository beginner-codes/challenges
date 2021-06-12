# Challenge 267 - It's a Meteor!

In a video game, a meteor will fall toward the main character's home planet. Given the meteor's trajectory as a string in the form `y = mx + b` and the character's position as a tuple of `(x, y)`, return `True` if the meteor will hit the character and `False` if it will not.

## Examples
```python
will_hit("y = 2x - 5", (0, 0)) ➞ False

will_hit("y = -4x + 6", (1, 2)) ➞ True

will_hit("y = 2x + 6", (3, 2)) ➞ False
```
## Notes

- The `b` value will never be zero or blank.
- The `m` value will always be an integer.
- If the `m` value is `1`, the `"1"` will be shown. For example, `"y = x + 5"` will be shown as `"y = 1x + 5"`.
- If the `m` value is `-1`, the `"-1"` will be shown. For example, `"y = -x + 2"` will be shown as `"y = -1x + 2"`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def will_hit(trajectory_slope: str, position: tuple[int, int]) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertFalse(will_hit("y = 2x - 5", (0, 0)))

    def test_2(self):
        self.assertTrue(will_hit("y = -4x + 6", (1, 2)))

    def test_3(self):
        self.assertFalse(will_hit("y = -4x + 6", (2, 2)))

    def test_4(self):
        self.assertTrue(will_hit("y = 3x - 8", (4, 4)))

    def test_5(self):
        self.assertFalse(will_hit("y = 2x + 6", (3, 2)))

    def test_6(self):
        self.assertTrue(will_hit("y = -3x + 15", (5, 0)))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Find The Largest Even Number](https://edabit.com/challenge/ksZrMdraPqHjvbaE6)
