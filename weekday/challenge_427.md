# Challenge 427 - A Pirate's Tale

Captain Hook and his crew are currently resting at Origin Shore. They are about to embark on their next adventure to an undisclosed location (x, y) to find treasure.

Captain Hook's ship can only move exactly north, south, east or west. It takes exactly 1 day for the ship to travel 1 unit in one of the four cardinal directions.

After every 5 days, the crew will take one day of rest.

Given the location of the treasure, find out how long it takes for Captain Hook and his crew to find the treasure. The ship is currently at coordinate (0, 0).
```python
number_of_days([3, 5]) => 9 days
# Since: 3 days east + 2 days north (5 days passed) + 1 day of rest + 3 days north

number_of_days([-4, -1]) => 5 days
# Since 4 days west + 1 day south
```
## Examples
```python
number_of_days([10, 10]) ➞ 23

number_of_days([3, 3]) ➞ 7

number_of_days([-10, -9]) ➞ 22

number_of_days([-1, -2]) ➞ 3
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from typing import Sequence
import unittest


Coord = Sequence[int, int]


def number_of_days(treasure: Coord) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(number_of_days([10, 10]), 23)

    def test_2(self):
        self.assertEqual(number_of_days([3, 3]), 7)

    def test_3(self):
        self.assertEqual(number_of_days([-10, -9]), 22)

    def test_4(self):
        self.assertEqual(number_of_days([-1, -4]), 5)

    def test_5(self):
        self.assertEqual(number_of_days([-10, -2]), 14)

    def test_6(self):
        self.assertEqual(number_of_days([3, 30]), 39)

    def test_7(self):
        self.assertEqual(number_of_days([40, 1]), 49)

    def test_8(self):
        self.assertEqual(number_of_days([3, 5]), 9)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [A Pirate's Tale](https://edabit.com/challenge/KNcoiggMPCXcj3aML)
