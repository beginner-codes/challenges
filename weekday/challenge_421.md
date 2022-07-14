# Challenge 421 - Scalable Mountain?

Given a list of numbers representing the height of a mountain at certain intervals, return whether this mountain is scalable.

A mountain can be considered scalable if each number is within 5 units of the next number in either direction.

## Examples
```python
is_scalable([1, 2, 4, 6, 7, 8]) ➞ True

is_scalable([40, 45, 50, 45, 47, 52]) ➞ True

is_scalable([2, 9, 11, 10, 18, 21]) ➞ False
```
## Notes

- The list may start at any number and can be any length.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def is_scalable(mountain: list[int]) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(is_scalable([1, 2, 4, 6, 7, 8]))

    def test_2(self):
        self.assertTrue(is_scalable([40, 45, 50, 48, 47, 52]))

    def test_3(self):
        self.assertFalse(is_scalable([2, 9, 11, 10, 18, 21]))

    def test_4(self):
        self.assertTrue(is_scalable([200, 200, 200, 200]))

    def test_5(self):
        self.assertTrue(is_scalable([30, 29, 24, 19, 16, 11]))

    def test_6(self):
        self.assertFalse(is_scalable([22, 22, 22, 29, 29, 29, 29]))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Scalable Mountain?](https://edabit.com/challenge/x3pW72MfFLi2GYh6g)
