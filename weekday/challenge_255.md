# Challenge 255 - Check If the Brick Fits through the Hole

Write the function that takes three dimensions of a brick: height, width, and depth and returns `True` if this brick can fit into a hole with the given width and height.

## Examples
```python
does_brick_fit(1, 1, 1, 1, 1) ➞ True

does_brick_fit(1, 2, 1, 1, 1) ➞ True

does_brick_fit(1, 2, 2, 1, 1) ➞ False
```
## Notes

- You can turn the brick with any side towards the hole.
- We assume that the brick fits if its sizes equal the ones of the hole (i.e. brick size should be less than or equal to the size of the hole, not strictly less).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def does_brick_fit(width: int, height: int, depth: int, hole_width: int, hole_height: int) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(does_brick_fit(1, 1, 1, 1, 1))

    def test_2(self):
        self.assertTrue(does_brick_fit(1, 2, 1, 1, 1))

    def test_3(self):
        self.assertFalse(does_brick_fit(1, 2, 2, 1, 1))

    def test_4(self):
        self.assertTrue(does_brick_fit(1, 2, 2, 1, 2))

    def test_5(self):
        self.assertTrue(does_brick_fit(1, 2, 2, 2, 1))

    def test_6(self):
        self.assertFalse(does_brick_fit(2, 2, 2, 1, 2))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Check If the Brick Fits through the Hole](https://edabit.com/challenge/ixdXLyopP7c4aPXqx)
