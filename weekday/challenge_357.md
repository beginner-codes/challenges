# Challenge 357 - Record Temperatures

You are given two lists that each contain data that represents the min and max weather temperatures for each day of the week.

The records list contains the all-time record low/high temperatures for that day of the week.
```python
[[record low, record high], ...]
```
The current week list contains the daily low/high temperatures for each day of the current week.
```python
[[daily low, daily high], ...]
```
A daily high temperature is considered a new record high if it is higher than the record high for that day of the week. A daily low temperature is considered a new record low if it is lower than the record low for that day of the week.

Compare the daily low/high temperatures of the current week to the record lows/highs and return a list with the updated record temperatures.

- There may be multiple record temperatures in a week.
- If there are no broken records return the original records list.

## Example
```python
#             sun       mon      tues       wed      thur      fri       sat
record_temps([[34, 82], [24, 82], [20, 89],  [5, 88],  [9, 88], [26, 89], [27, 83]],
            [[44, 72], [19, 70], [40, 69], [39, 68], [33, 64], [36, 70], [38, 69]])

➞           [[34, 82], [19, 82], [20, 89], [5, 88], [9, 88], [26, 89], [27, 83]]
# The previous record low for Monday was 24. The current week's low for Monday was 19. So 19 replaces 24 as Monday's new record low.
```
## Notes

- There won't be a record high and record low set on the same day.
- Index `0` will always be the low and index `1` will always be the high `[low, high]`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


LOW_HIGH = list[int, int]
WEEK = list[LOW_HIGH, LOW_HIGH, LOW_HIGH, LOW_HIGH, LOW_HIGH, LOW_HIGH, LOW_HIGH]


def record_temps(*records: WEEK) -> WEEK:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(
            record_temps(
                [[34, 82], [24, 82], [20, 89], [5, 88], [9, 88], [26, 89], [27, 83]],
                [[44, 72], [19, 70], [40, 69], [39, 68], [33, 64], [36, 70], [38, 69]],
            ),
            [[34, 82], [19, 82], [20, 89], [5, 88], [9, 88], [26, 89], [27, 83]],
        )

    def test_2(self):
        self.assertListEqual(
            record_temps(
                [
                    [25, 80],
                    [27, 88],
                    [19, 88],
                    [23, 85],
                    [21, 89],
                    [23, 78],
                    [17, 79],
                ],
                [
                    [40, 70],
                    [41, 68],
                    [45, 68],
                    [39, 65],
                    [44, 72],
                    [43, 69],
                    [37, 68],
                ],
            ),
            [
                [25, 80],
                [27, 88],
                [19, 88],
                [23, 85],
                [21, 89],
                [23, 78],
                [17, 79],
            ],
        )

    def test_3(self):
        self.assertListEqual(
            record_temps(
                [
                    [19, 78],
                    [21, 79],
                    [22, 90],
                    [21, 79],
                    [30, 86],
                    [25, 82],
                    [19, 80],
                ],
                [
                    [29, 68],
                    [24, 69],
                    [28, 63],
                    [20, 50],
                    [25, 65],
                    [28, 56],
                    [30, 61],
                ],
            ),
            [
                [19, 78],
                [21, 79],
                [22, 90],
                [20, 79],
                [25, 86],
                [25, 82],
                [19, 80],
            ],
        )

    def test_4(self):
        self.assertListEqual(
            record_temps(
                [
                    [29, 90],
                    [19, 78],
                    [26, 91],
                    [20, 86],
                    [29, 79],
                    [16, 84],
                    [24, 83],
                ],
                [
                    [33, 68],
                    [38, 58],
                    [36, 59],
                    [40, 56],
                    [37, 69],
                    [39, 70],
                    [41, 69],
                ],
            ),
            [
                [29, 90],
                [19, 78],
                [26, 91],
                [20, 86],
                [29, 79],
                [16, 84],
                [24, 83],
            ],
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Record Temperatures](https://edabit.com/challenge/rix73vi9mFYWWqPoA)
