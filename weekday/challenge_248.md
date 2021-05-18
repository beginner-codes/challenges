# Challenge 248 - Convenience Store

Given a total due and a list representing the amount of change in your pocket, determine whether you are able to pay for the item. Change will always be represented in the following order: quarters, dimes, nickels, pennies.

To illustrate: `has_enough_change([25, 20, 5, 0], 4.25)` should return `True`, since having 25 quarters, 20 dimes, 5 nickels and 0 pennies gives you `6.25 + 2 + .25 + 0 = 8.50`.

## Examples
```python
has_enough_change([2, 100, 0, 0], 14.11) ➞ False

has_enough_change([0, 0, 20, 5], 0.75) ➞ True

has_enough_change([30, 40, 20, 5], 12.55) ➞ True

has_enough_change([10, 0, 0, 50], 3.85) ➞ False

has_enough_change([1, 0, 5, 219], 19.99) ➞ False
```
## Notes

- quarter: 25 cents / $0.25
- dime: 10 cents / $0.10
- nickel: 5 cents / $0.05
- penny: 1 cent / $0.01

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def has_enough_change(change: list[int], total: float) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertFalse(has_enough_change([2, 100, 0, 0], 14.11))

    def test_2(self):
        self.assertTrue(has_enough_change([0, 0, 20, 5], 0.75))

    def test_3(self):
        self.assertTrue(has_enough_change([30, 40, 20, 5], 12.55))

    def test_4(self):
        self.assertFalse(has_enough_change([10, 0, 0, 50], 13.85))

    def test_5(self):
        self.assertFalse(has_enough_change([1, 0, 5, 219], 19.99))

    def test_6(self):
        self.assertTrue(has_enough_change([1, 0, 2555, 219], 127.75))

    def test_7(self):
        self.assertTrue(has_enough_change([1, 335, 0, 219], 35.21))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Convenience Store](https://edabit.com/challenge/erFxBbqzZPSegMwnc)
