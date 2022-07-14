# Challenge 428 - Shopping for Memorial Day!

Create a function that takes a list of objects and calculate the total based on the quantity of items purchased. Apply a 6% sales tax for each item when appropriate.

## Examples
```python
checkout([
  { "desc": "potato chips", "prc": 2, "qty": 2, "taxable": false },
  { "desc": "soda", "prc": 3, "qty": 2, "taxable": false },
  { "desc": "paper plates", "prc": 5, "qty": 1, "taxable": true }
]) ➞ 15.3
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from typing import TypedDict
import unittest


Item = TypedDict("Item", {"desc": str, "prc": int, "qty": int, "taxable": bool})


def checkout(items: list[Item]) -> float:
    return 0.0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(
            checkout(
                [
                    {"desc": "grill", "prc": 300, "qty": 1, "taxable": True},
                    {"desc": "hotdogs", "prc": 10, "qty": 2, "taxable": False},
                    {"desc": "US Flag", "prc": 30, "qty": 1, "taxable": True},
                ]
            ),
            369.8,
        )

    def test_2(self):
        self.assertEqual(
            checkout(
                [
                    {"desc": "hamburger", "prc": 5, "qty": 2, "taxable": False},
                    {"desc": "potato salad", "prc": 8, "qty": 1, "taxable": False},
                    {"desc": "potato chips", "prc": 2, "qty": 2, "taxable": False},
                    {"desc": "soda", "prc": 3, "qty": 2, "taxable": False},
                    {"desc": "paper plates", "prc": 5, "qty": 1, "taxable": True},
                ]
            ),
            33.3,
        )

    def test_3(self):
        self.assertEqual(
            checkout(
                [
                    {"desc": "beach umbrella", "prc": 58, "qty": 1, "taxable": True},
                    {"desc": "beach towel", "prc": 9, "qty": 2, "taxable": True},
                    {"desc": "swim suit", "prc": 25, "qty": 2, "taxable": False},
                    {"desc": "soda", "prc": 3, "qty": 2, "taxable": False},
                    {"desc": "cooler", "prc": 25, "qty": 1, "taxable": True},
                ]
            ),
            163.06,
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Shopping for Memorial Day!](https://edabit.com/challenge/jgrDqqNm8z2kzJ6mH)
