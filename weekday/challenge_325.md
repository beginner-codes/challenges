# Challenge 325 - Bundle Up!

Lets assume for the purposes of this challenge that for every layer of fabric you wear when it's cold outside (coats, cardigans, etc), the temperature increases by a tenth of the total.

Given n number of layers and a given temperature, write a function that returns the temperature inside of all those warm fuzzy layers. Round to the nearest tenth of a degree.
```python
calc_bundled_temp(2, "10*C") ➞ "12.1*C"
# 10 * 1.1 = 11
# 11 * 1.1 = 12.1
```
## Examples
```python
calc_bundled_temp(1, "2*C") ➞ "2.2*C"

calc_bundled_temp(4, "6*C") ➞ "8.8*C"

calc_bundled_temp(20, "4*C") ➞ "26.9*C"
```
## Notes

- The temperature will be given in celsius and as a string.
- Note that the degrees sign is given as an asterisk.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def calc_bundled_temp(layers: int, temperature: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(calc_bundled_temp(2, "10*C"), "12.1*C")

    def test_2(self):
        self.assertEqual(calc_bundled_temp(1, "2*C"), "2.2*C")

    def test_3(self):
        self.assertEqual(calc_bundled_temp(4, "6*C"), "8.8*C")

    def test_4(self):
        self.assertEqual(calc_bundled_temp(20, "4*C"), "26.9*C")

    def test_5(self):
        self.assertEqual(calc_bundled_temp(5, "20*C"), "32.2*C")

    def test_6(self):
        self.assertEqual(calc_bundled_temp(20, "3*C"), "20.2*C")

    def test_7(self):
        self.assertEqual(calc_bundled_temp(5, "18*C"), "29.0*C")

    def test_8(self):
        self.assertEqual(calc_bundled_temp(4, "5*C"), "7.3*C")

    def test_9(self):
        self.assertEqual(calc_bundled_temp(16, "17*C"), "78.1*C")

    def test_10(self):
        self.assertEqual(calc_bundled_temp(15, "2*C"), "8.4*C")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Bundle Up!](https://edabit.com/challenge/qKAcMAkWXvXKAxXut)
