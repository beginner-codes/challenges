# Challenge 347 - Reversing a Binary Integer

Write a function that takes an integer, reverses the binary representation of that integer, and returns the new integer from the reversed binary.

## Examples
```python
reversed_binary_integer(10) ➞ 5
# 10 = 1010 -> 0101 = 5

reversed_binary_integer(12) ➞ 3
# 12 = 1100 -> 0011 = 3

reversed_binary_integer(25) ➞ 19
# 25 = 11001 -> 10011 = 19

reversed_binary_integer(45) ➞ 45
# 45 = 101101 -> 101101 = 45
```
## Notes

- All values will be positive.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def reversed_binary_integer(integer: int) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(reversed_binary_integer(1), 1)

    def test_2(self):
        self.assertEqual(reversed_binary_integer(4), 1)

    def test_3(self):
        self.assertEqual(reversed_binary_integer(5), 5)

    def test_4(self):
        self.assertEqual(reversed_binary_integer(31), 31)

    def test_5(self):
        self.assertEqual(reversed_binary_integer(82), 37)

    def test_6(self):
        self.assertEqual(reversed_binary_integer(90), 45)

    def test_7(self):
        self.assertEqual(reversed_binary_integer(255), 255)

    def test_8(self):
        self.assertEqual(reversed_binary_integer(446), 251)

    def test_9(self):
        self.assertEqual(reversed_binary_integer(451), 391)

    def test_10(self):
        self.assertEqual(reversed_binary_integer(634), 377)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Reversing a Binary String](https://edabit.com/challenge/WPojigJER35bJT6YH)
