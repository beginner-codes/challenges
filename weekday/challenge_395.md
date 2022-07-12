# Challenge 395 - How Many Rectangles?

Let there be a square matrix, where each square is a rectangle, and a combination of more squares are also rectangles. To find the number of rectangles, Pete sat down and started counting... but that's highly inefficient.

Create a function that takes the order of the matrix as input and returns the number of rectangles in them.

## Examples
```python
rectangles(1) ➞ 1

rectangles(2) ➞ 9

rectangles(3) ➞ 36
```
## Notes

- The input will always be an integer.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def rectangles(matrix_size: int) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(rectangles(64), 4326400)

    def test_2(self):
        self.assertEqual(rectangles(76), 8561476)

    def test_3(self):
        self.assertEqual(rectangles(10), 3025)

    def test_4(self):
        self.assertEqual(rectangles(79), 9985600)

    def test_5(self):
        self.assertEqual(rectangles(84), 12744900)

    def test_6(self):
        self.assertEqual(rectangles(0), 0)

    def test_7(self):
        self.assertEqual(rectangles(60), 3348900)

    def test_8(self):
        self.assertEqual(rectangles(29), 189225)

    def test_9(self):
        self.assertEqual(rectangles(18), 29241)

    def test_10(self):
        self.assertEqual(rectangles(74), 7700625)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [How Many Rectangles?](https://edabit.com/challenge/zRm6YDfQHoesdc3rb)
