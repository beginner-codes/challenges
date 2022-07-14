# Challenge 364 - Number of Leap Years

Given a range of years as a string, create a function that returns the number of leap years there are within the range (inclusive).

## Examples
```python
num_of_leapyears("1980-1984") ➞ 2
# 1980 and 1984 are leapyears.

num_of_leapyears("2000-2020") ➞ 6

num_of_leapyears("1600-2000") ➞ 98
```
## Notes

- Remember that a hyphen separates the years.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def number_of_leapyears(years: str) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(num_of_leapyears("2000-2020"), 6)

    def test_2(self):
        self.assertEqual(num_of_leapyears("1600-2000"), 98)

    def test_3(self):
        self.assertEqual(num_of_leapyears("1980-1984"), 2)

    def test_4(self):
        self.assertEqual(num_of_leapyears("1224-8090"), 1666)

    def test_5(self):
        self.assertEqual(num_of_leapyears("2486-7607"), 1241)

    def test_6(self):
        self.assertEqual(num_of_leapyears("1813-4354"), 616)

    def test_7(self):
        self.assertEqual(num_of_leapyears("772-1849"), 262)

    def test_8(self):
        self.assertEqual(num_of_leapyears("2228-7099"), 1182)

    def test_9(self):
        self.assertEqual(num_of_leapyears("1349-6325"), 1206)

    def test_10(self):
        self.assertEqual(num_of_leapyears("1803-3828"), 492)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Number of Leap Years](https://edabit.com/challenge/xCXdch4XLpXZZagxm)
