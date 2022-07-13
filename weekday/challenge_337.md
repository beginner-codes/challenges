# Challenge 337 - Sort the Dates

In this challenge, create a function to sort a list containing a series of dates given as strings. Each date is given in the format `DD-MM-YYYY_HH:MM`:
```
"12-02-2012_13:44"
```
The priority of criteria used for sorting will be:

1. Year
2. Month
3. Day
4. Hours
5. Minutes

6. Given a list and a ordering mode, implement a function that returns:

- if mode is equal to `"ASC"`, the list sorted in ascending order.
- if mode is equal to `"DSC"`, the list sorted in descending order.

## Examples
```python
sort_dates(["10-02-2018_12:30", "10-02-2016_12:30", "10-02-2018_12:15"], "ASC") ➞ ["10-02-2016_12:30", "10-02-2018_12:15", "10-02-2018_12:30"]

sort_dates(["10-02-2018_12:30", "10-02-2016_12:30", "10-02-2018_12:15"], "DSC") ➞ ["10-02-2018_12:30", "10-02-2018_12:15", "10-02-2016_12:30"]

sort_dates(["09-02-2000_10:03", "10-02-2000_18:29", "01-01-1999_00:55"], "ASC") ➞ ["01-01-1999_00:55", "09-02-2000_10:03", "10-02-2000_18:29"]
```
## Notes

- Remember: the date is in the format `DD-MM-YYYY_HH:MM`.
- You can expect only valid formatted dates, without exceptions to handle.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def sort_dates(dates: list[str], ordering: str) -> list[str]:
    return []  # Put your code here!!!


dates1 = [
    "18-10-2016_12:09",
    "01-12-2017_20:32",
    "18-10-2016_12:04",
    "19-10-2017_16:20",
    "18-10-2017_16:19",
    "18-10-2016_16:19",
]

dates2 = [
    "11-02-2011_00:01",
    "21-04-2013_11:43",
    "02-09-2018_11:00",
    "02-09-2018_10:00",
    "02-09-2018_10:30",
    "11-02-2011_00:00",
]


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(
            sort_dates(dates1, "ASC"),
            [
                "18-10-2016_12:04",
                "18-10-2016_12:09",
                "18-10-2016_16:19",
                "18-10-2017_16:19",
                "19-10-2017_16:20",
                "01-12-2017_20:32",
            ],
        )

    def test_2(self):
        self.assertListEqual(
            sort_dates(dates1, "DSC"),
            [
                "01-12-2017_20:32",
                "19-10-2017_16:20",
                "18-10-2017_16:19",
                "18-10-2016_16:19",
                "18-10-2016_12:09",
                "18-10-2016_12:04",
            ],
        )

    def test_3(self):
        self.assertListEqual(
            sort_dates(dates2, "DSC"),
            [
                "02-09-2018_11:00",
                "02-09-2018_10:30",
                "02-09-2018_10:00",
                "21-04-2013_11:43",
                "11-02-2011_00:01",
                "11-02-2011_00:00",
            ],
        )

    def test_4(self):
        self.assertListEqual(
            sort_dates(dates2, "ASC"),
            [
                "11-02-2011_00:00",
                "11-02-2011_00:01",
                "21-04-2013_11:43",
                "02-09-2018_10:00",
                "02-09-2018_10:30",
                "02-09-2018_11:00",
            ],
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Sort the Dates](https://edabit.com/challenge/whmsRve8YQ23wZuh4)
