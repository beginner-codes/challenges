# Challenge 224 - Power Ranger

Create a function that takes power, lower, and upper and returns the number of positive values raised to the nth power that lie in the range `[a, b]`, inclusive.

## Examples
```python
power_ranger(2, 49, 65) ➞ 2
# 2 squares (n^2) lie between 49 and 65, 49 (7^2) and 64 (8^2)

power_ranger(3, 1, 27) ➞ 3
# 3 cubes (n^3) lie between 1 and 27, 1 (1^3), 8 (2^3) and 27 (3^3)

power_ranger(10, 1, 5) ➞ 1
# 1 value raised to the 10th power lies between 1 and 5, 1 (1^10)

power_ranger(5, 31, 33) ➞ 1

power_ranger(4, 250, 1300) ➞ 3
```
## Notes

- Remember that the range is inclusive.
- `a < b` will always be true.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def power_ranger(power: int, lower: int, upper: int) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(power_ranger(5, 31, 33), 1)

    def test_2(self):
        self.assertEqual(power_ranger(4, 250, 1300), 3)

    def test_3(self):
        self.assertEqual(power_ranger(2, 49, 65), 2)

    def test_4(self):
        self.assertEqual(power_ranger(3, 1, 27), 3)

    def test_5(self):
        self.assertEqual(power_ranger(10, 1, 5), 1)

    def test_6(self):
        self.assertEqual(power_ranger(1, 1, 5), 5)

    def test_7(self):
        self.assertEqual(power_ranger(2, 1, 100), 10)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Power Ranger](https://edabit.com/challenge/abdsaD6gwjgAgevsG)
