# Challenge 200 - Free Throw Probability

To train for an upcoming marathon, Johnny goes on one long-distance run each Saturday. He wants to track how often the number of miles he runs exceeds the previous Saturday. This is called a progress day.

Create a function that takes in a list of miles run every Saturday and returns Johnny's total number of progress days.

## Examples
```python
progress_days([3, 4, 1, 2]) ➞ 2
# There are two progress days, (3->4) and (1->2)

progress_days([10, 11, 12, 9, 10]) ➞ 3

progress_days([6, 5, 4, 3, 2, 9]) ➞ 1

progress_days([9, 9])  ➞ 0
```
## Notes

- Running the same number of miles as last week does not count as a progress day.  

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def progress_days(saturdays: list[int]) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(progress_days([3, 4, 1, 2]), 2)

    def test_2(self):
        self.assertEqual(progress_days([10, 11, 12, 9, 10]), 3)

    def test_3(self):
        self.assertEqual(progress_days([6, 5, 4, 3, 2, 9]), 1)

    def test_4(self):
        self.assertEqual(progress_days([9, 9]), 0)

    def test_5(self):
        self.assertEqual(progress_days([12, 11, 10, 12, 11, 13]), 2)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Is Johnny Making Progress?](https://edabit.com/challenge/2yHQwkecEHZBfHcmN)
