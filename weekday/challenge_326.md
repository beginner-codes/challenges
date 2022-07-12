# Challenge 326 - Crowded Carriage Capacity

A train has a maximum capacity of passengers overall, which means each carriage's capacity will share an equal proportion of the maximum capacity.

Create a function which returns the index of the first carriage which holds 50% or less of its maximum capacity. If no such carriage exists, return -1.

__Worked Example__
```python
find_a_seat(200, [35, 23, 18, 10, 40]) ➞ 2

# There are 5 carriages which each have a maximum capacity of 40 (200 / 5 = 40).
# Index 0's carriage is too full (35 is 87.5% of the maximum).
# Index 1's carriage is too full (23 is 57.5% of the maximum).
# Index 2's carriage is good enough (18 is 45% of the maximum).
# Return 2.
```
## Examples
```python
find_a_seat(20, [3, 5, 4, 2]) ➞ 3

find_a_seat(1000, [50, 20, 80, 90, 100, 60, 30, 50, 80, 60]) ➞ 0

find_a_seat(200, [35, 23, 40, 21, 38]) ➞ -1
```
## Notes

- This means if a train can hold 200 passengers, and has 5 carriages, then that means each carriage can hold a maximum of 40 passengers each (200 / 5 = 40.
- All carriage numbers will be positive integers, which will be able to divide evenly.
- Remember to return `-1` if no carriage is empty enough.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def find_a_seat(max_capacity: int, car_occupancies: list[int]) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(find_a_seat(20, [3, 5, 4, 2]), 3)

    def test_2(self):
        self.assertEqual(find_a_seat(1000, [50, 20, 80, 90, 100, 60, 30, 50, 80, 60]), 0)

    def test_3(self):
        self.assertEqual(find_a_seat(200, [35, 23, 40, 21, 38]), -1)

    def test_4(self):
        self.assertEqual(find_a_seat(200, [35, 23, 18, 10, 40]), 2)

    def test_5(self):
        self.assertEqual(find_a_seat(21, [6, 3, 7]), 1)

    def test_6(self):
        self.assertEqual(find_a_seat(11037, [1839, 0, 0]), 0)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Crowded Carriage Capacity](https://edabit.com/challenge/XfSvKco6KZFRfgQyj)
