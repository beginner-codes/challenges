# Challenge 266 - Find The Largest Even Number

Write a function that finds the largest even number in a list. Return -1 if not found.

## Examples
```python
largest_even([3, 7, 2, 1, 7, 9, 10, 13]) ➞ 10

largest_even([1, 3, 5, 7]) ➞ -1

largest_even([0, 19, 18973623]) ➞ 0
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def largest_even(numbers: list[int]) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(largest_even([3, 7, 2, 1, 7, 9, 10, 13]), 10)

    def test_2(self):
        self.assertEqual(largest_even([1]), -1)

    def test_3(self):
        self.assertEqual(largest_even([22]), 22)

    def test_4(self):
        self.assertEqual(largest_even([13, 5, 7, 9]), -1)

    def test_5(self):
        self.assertEqual(largest_even([3, 19, 18973623, 2]), 2)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Find The Largest Even Number](https://edabit.com/challenge/ksZrMdraPqHjvbaE6)
