# Challenge 391 - Does the Cargo Fit?

A ship has to transport cargo from one place to another, while picking up cargo along the way. Given the total amount of cargo and the types of cargo holds in the ship as lists, create a function that returns `True` if all the cargo can fit on the ship, and `False` if it can't.

- `"S"` means 50 cargo space.
- `"M"` means 100 cargo space.
- `"L"` means 200 cargo space.

## Examples
```python
will_fit(["M", "L", "L", "M"], [56, 62, 84, 90]) ➞ True

will_fit(["S", "S", "S", "S", "L"], [40, 50, 60, 70 , 80, 90, 200]) ➞ False

will_fit(["L", "L", "M"], [56, 62, 84, 90]) ➞ True
```
## Notes

- Calculate the cargo as a whole, and not for each separate cargo hold

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def will_fit(num_people: int) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(will_fit(["M", "L", "L", "M"], [56, 62, 84, 90]))

    def test_2(self):
        self.assertTrue(will_fit(["L", "L", "M"], [56, 62, 84, 90]))

    def test_3(self):
        self.assertFalse(
            will_fit(["S", "S", "S", "S", "L"], [40, 50, 60, 70, 80, 90, 200])
        )

    def test_4(self):
        self.assertFalse(will_fit(["S", "L"], [73, 87, 95, 229]))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Does the Cargo Fit? (Part 1)](https://edabit.com/challenge/ziaNsc7J4ySFY6rF6)
