# Challenge 336 - How Many Days Between Two Dates

Create a function that takes two dates and returns the number of days between the first and second date.

## Examples
```python
get_days(
  datetime.date(2019, 6, 14),  # June 14, 2019
  datetime.date(2019, 6, 20)  # June 20, 2019
) ➞ 6


get_days(
  datetime.date(2018, 12, 29),  # December 29, 2018
  datetime.date(2019, 1, 1)  # January 1, 2019
) ➞ 3
# Dates may not all be in the same month/year.

get_days(
  datetime.date(2020, 5, 24),
  datetime.date(2019, 5, 24))
) ➞ -366
# Backwards dates should return a negative change.
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from datetime import date
import unittest


def get_days(date_a: date, date_b: date) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(get_days(date(2019, 6, 14), date(2019, 6, 20)), 6)

    def test_2(self):
        self.assertEqual(get_days(date(2018, 12, 29), date(2019, 1, 1)), 3)

    def test_3(self):
        self.assertEqual(get_days(date(2019, 7, 20), date(2019, 7, 30)), 10)

    def test_4(self):
        self.assertEqual(get_days(date(2020, 5, 24), date(2020, 9, 25)), 124)

    def test_5(self):
        self.assertEqual(get_days(date(2020, 5, 24), date(2019, 5, 24)), -366)

    def test_6(self):
        self.assertEqual(get_days(date(2020, 4, 30), date(1963, 11, 23)), -20613)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [How Many Days Between Two Dates](https://edabit.com/challenge/YSikG4DEsnxahg2u4)
