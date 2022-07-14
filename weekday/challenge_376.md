# Challenge 376 - Divisible by Left Digit?

Create a function that takes a number and checks if each digit is divisible by the digit on its left. Return a boolean list of the condition checks.

## Examples
```python
divisible_by_left(73312) ➞ [False, False, True, False, True]
# no element left to 7 = False
# 3/7 = False
# 3/3 = True
# 1/3 = False
# 2/1 = True

divisible_by_left(1) ➞ [False]

divisible_by_left(635) ➞ [False, False, False]
```
## Notes

- The array should always start with False as there is no digit to the left of the first digit.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def divisible_by_left(number: int) -> list[bool]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(divisible_by_left(1), [False])

    def test_2(self):
        self.assertListEqual(divisible_by_left(1248), [False, True, True, True])

    def test_3(self):
        self.assertListEqual(divisible_by_left(4321), [False, False, False, False])

    def test_4(self):
        self.assertListEqual(
            divisible_by_left(73312), [False, False, True, False, True]
        )

    def test_5(self):
        self.assertListEqual(divisible_by_left(2026), [False, True, False, True])

    def test_6(self):
        self.assertListEqual(divisible_by_left(635), [False, False, False])

    def test_7(self):
        self.assertListEqual(divisible_by_left(1337), [False, True, True, False])

    def test_8(self):
        self.assertListEqual(
            divisible_by_left(135028), [False, True, False, True, False, True]
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Divisible by Left Digit?](https://edabit.com/challenge/wsCshmu5zkN5BfeAC)
