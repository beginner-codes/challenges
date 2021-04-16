# Challenge 226 - Get Free Wi-Fi Anywhere You Go

A new 'hacky' phone is launched, which has the feature of connecting to any Wi-Fi network from any distance away, as long as there aren't any obstructions between the hotspot and the phone. Given a string, return how many Wi-Fi hotspots I'm able to connect to.

- The phone is represented as a `P`.
- A hotspot is represented as an `*`.
- An obstruction is represented as a `#`.
  
You cannot access a hotspot if it is behind an obstruction.

## Examples
```python
nonstop_hotspot("*   P  *   *") ➞ 3

nonstop_hotspot("*  * #  * P # * #") ➞ 1

nonstop_hotspot("***#P#***") ➞ 0
```
## Notes

- There will be only one phone.
- No other characters, other than spaces, will appear in the tests.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def digit_occurrences(start: int, end: int, match: int) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(digit_occurrences(51, 55, 5), 6)

    def test_2(self):
        self.assertEqual(digit_occurrences(1, 8, 9), 0)

    def test_3(self):
        self.assertEqual(digit_occurrences(71, 77, 2), 1)

    def test_4(self):
        self.assertEqual(digit_occurrences(1, 14, 4), 2)

    def test_5(self):
        self.assertEqual(digit_occurrences(20, 30, 2), 11)

    def test_6(self):
        self.assertEqual(digit_occurrences(18, 37, 3), 10)

    def test_7(self):
        self.assertEqual(digit_occurrences(5, 335, 6), 63)

    def test_8(self):
        self.assertEqual(digit_occurrences(-19, 19, 0), 3)

    def test_9(self):
        self.assertEqual(digit_occurrences(-8, -1, 8), 1)

    def test_10(self):
        self.assertEqual(digit_occurrences(-5, -5, 4), 0)

    def test_11(self):
        self.assertEqual(digit_occurrences(-5, -5, 5), 1)

    def test_12(self):
        self.assertEqual(digit_occurrences(-50, -45, 4), 5)

    def test_13(self):
        self.assertEqual(digit_occurrences(-500, -45, 4), 190)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Count a Specific Digit](https://edabit.com/challenge/tNRvtHKZxvqPRnAeF)
