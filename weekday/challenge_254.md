# Challenge 254 - Find the nth Tetrahedral Number

A tetrahedron is a pyramid with a triangular base and three sides. A tetrahedral number is a number of items within a tetrahedron.

Create a function that takes an integer and returns the nth tetrahedral number.

## Examples
```python
get_nth_tetrahedral(2) ➞ 4

get_nth_tetrahedral(5) ➞ 35

get_nth_tetrahedral(6) ➞ 56
```
## Notes

- There is a formula for the nth tetrahedral number.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def get_nth_tetrahedral(nth: int) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(get_nth_tetrahedral(1), 1)

    def test_2(self):
        self.assertEqual(get_nth_tetrahedral(2), 4)

    def test_3(self):
        self.assertEqual(get_nth_tetrahedral(3), 10)

    def test_4(self):
        self.assertEqual(get_nth_tetrahedral(4), 20)

    def test_5(self):
        self.assertEqual(get_nth_tetrahedral(5), 35)

    def test_6(self):
        self.assertEqual(get_nth_tetrahedral(9), 165)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Find the nth Tetrahedral Number](https://edabit.com/challenge/zRCyxKBBmr4F2x4Bv)
