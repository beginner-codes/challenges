# Challenge 321 - Largest Gap

Write a function that given a list of integers, returns the largest gap between elements of the sorted list.

Here's an illustrative example. Consider the list:
```python
[9, 4, 26, 26, 0, 0, 5, 20, 6, 25, 5]
```
... which, after sorting, becomes the list:
```python
[0, 0, 4, 5, 5, 6, 9, 20, 25, 26, 26]
```
... so that we now see that the largest gap in the list is the gap of 11 between 9 and 20.

## Examples
```python
largest_gap([9, 4, 26, 26, 0, 0, 5, 20, 6, 25, 5]) ➞ 11
# After sorting get [0, 0, 4, 5, 5, 6, 9, 20, 25, 26, 26]
# Largest gap of 11 between 9 and 20

largest_gap([14, 13, 7, 1, 4, 12, 3, 7, 7, 12, 11, 5, 7]) ➞ 4
# After sorting get [1, 3, 4, 5, 7, 7, 7, 7, 11, 12, 12, 13, 14]
# Largest gap of 4 between 7 and 11

largest_gap([13, 3, 8, 5, 5, 2, 13, 6, 14, 2, 11, 4, 10, 8, 1, 9]) ➞ 2
# After sorting get [1, 2, 2, 3, 4, 5, 5, 6, 8, 8, 9, 10, 11, 13, 13, 14]
# Largest gap of 2 between 6 and 8
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def largest_gap(numbers: list[int]) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(largest_gap([9, 4, 26, 26, 0, 0, 5, 20, 6, 25, 5]), 11)

    def test_2(self):
        self.assertEqual(largest_gap([14, 13, 7, 1, 4, 12, 3, 7, 7, 12, 11, 5, 7]), 4)

    def test_3(self):
        self.assertEqual(
            largest_gap([1, 2, 2, 3, 4, 5, 5, 6, 8, 8, 9, 10, 11, 13, 13, 14]), 2
        )

    def test_4(self):
        self.assertEqual(largest_gap([21, 28, 0, 5, 11, 6, 17, 25, 2, 19]), 6)

    def test_5(self):
        self.assertEqual(largest_gap([8, 11, 24, 2, 7, 4, 4, 25, 24, 14, 8, 0, 7]), 10)

    def test_6(self):
        self.assertEqual(
            largest_gap(
                [26, 17, 4, 25, 29, 26, 8, 30, 4, 20, 2, 7, 29, 7, 20, 30, 23, 5]
            ),
            9,
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Largest Gap](https://edabit.com/challenge/qbCavpBpk8KSWM37s)
