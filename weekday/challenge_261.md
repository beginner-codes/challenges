# Challenge 261 - Perimeters

Write a function that takes a number and returns the perimeter of either a circle, a square, or an equilateral triangle. The input will be in the form letter and number, where the letter will be either `"s"` for square, `"c"` for circle, or `"t"` for triangle, and the number will be the side of the square/triangle or the radius of the circle.

Use the following formulas:

- Perimeter of a square: `4 * side`
- Perimeter of a circle: `π * radius`
- Perimeter of a triangle: `3 * side`

## Examples
```python
perimeter("s7") ➞ 28

perimeter("c4") ➞ 25.12

perimeter("t9") ➞ 27
```
## Notes

- Round to 2 decimal places

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def perimeter(details: str) -> float:
    return 0.0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertAlmostEqual(perimeter("s1"), 4, 2)

    def test_2(self):
        self.assertAlmostEqual(perimeter("s4"), 16, 2)

    def test_3(self):
        self.assertAlmostEqual(perimeter("s9"), 36, 2)

    def test_4(self):
        self.assertAlmostEqual(perimeter("s13"), 52, 2)

    def test_5(self):
        self.assertAlmostEqual(perimeter("s30"), 120, 2)

    def test_6(self):
        self.assertAlmostEqual(perimeter("c1"), 6.28, 2)

    def test_7(self):
        self.assertAlmostEqual(perimeter("c4"), 25.12, 2)

    def test_8(self):
        self.assertAlmostEqual(perimeter("c9"), 56.52, 2)

    def test_9(self):
        self.assertAlmostEqual(perimeter("c13"), 81.64, 2)

    def test_10(self):
        self.assertAlmostEqual(perimeter("c30"), 188.4, 2)

    def test_11(self):
        self.assertAlmostEqual(perimeter("t1"), 3, 2)

    def test_12(self):
        self.assertAlmostEqual(perimeter("t5"), 15, 2)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Adapted from Edabit: [Perimeters with a Catch](https://edabit.com/challenge/WEvqZTFcHeYzFn74c)
