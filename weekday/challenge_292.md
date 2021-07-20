# Challenge 292 - Paint the Walls

Given a predetermined rate from a dictionary, write the function that will return the time it takes for a certain number of people to paint a certain amount of walls. Return the minutes as an integer. No rounding is necessary.

## Example
```python
# It takes 22 minutes for 10 people to paint 10 walls.
# How many minutes does it take 14 people to paint 14 walls?

rate = {
  "people": 10,
  "walls": 10,
  "minutes": 22
}

time(rate, people, walls) ➞ 22
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def time(rate: dict[str, int], people: int, minutes: int) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        rate1 = {"people": 4, "walls": 9, "minutes": 63}
        self.assertEqual(time(rate1, 7, 4), 16)

    def test_2(self):
        rate2 = {"people": 10, "walls": 10, "minutes": 22}
        self.assertEqual(time(rate2, 10, 10), 22)

    # Original JavaScript challenge by Isaac Pak.


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Paint the Walls](https://edabit.com/challenge/W8imhL66osEpK2ANs)
