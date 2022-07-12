# Challenge 311 - Squares and Cubes

Create a function that takes a list of two numbers and checks if the square root of the first number is equal to the cube root of the second number.

## Examples
```python
check_square_and_cube([4, 8]) ➞ True

check_square_and_cube([16, 48]) ➞ False

check_square_and_cube([9, 27]) ➞ True
```
## Notes

- Remember to return either `True` or `False`.
- All lists contain two positive numbers.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def check_square_and_cube(numbers: list[int]) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(check_square_and_cube([4, 8]))

    def test_2(self):
        self.assertFalse(check_square_and_cube([5, 12]))

    def test_3(self):
        self.assertTrue(check_square_and_cube([9, 27]))

    def test_4(self):
        self.assertFalse(check_square_and_cube([25, 120]))

    def test_5(self):
        self.assertTrue(check_square_and_cube([25, 125]))

    def test_6(self):
        self.assertFalse(check_square_and_cube([36, 215]))

    def test_7(self):
        self.assertFalse(check_square_and_cube([36, 217]))

    def test_8(self):
        self.assertTrue(check_square_and_cube([144, 1728]))

    def test_9(self):
        self.assertTrue(check_square_and_cube([1, 1]))

    def test_10(self):
        self.assertTrue(check_square_and_cube([676, 17576]))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Squares and Cubes](https://edabit.com/challenge/NMHFTCMqW6j8sXkNd)
