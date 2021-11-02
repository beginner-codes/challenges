# Challenge 365 - Slidey Numbers

Write a function that takes a number and determines if it is "slidey." A number is considered slidey if for every digit in the number, the next digit from that has an absolute difference of one. Check the examples below.

## Examples
```python
is_slidey(123454321) ➞ True

is_slidey(54345) ➞ True

is_slidey(987654321) ➞ True

is_slidey(1123) ➞ False

is_slidey(1357) ➞ False
```
## Notes

- A number cannot slide properly if there is a "flat surface" (example #4), or has gaps (example #5).
- All single digit numbers can be considered slidey numbers!

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def is_slidey(number: int) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(is_slidey(123454321))

    def test_2(self):
        self.assertTrue(is_slidey(54345))

    def test_3(self):
        self.assertTrue(is_slidey(987654321))

    def test_4(self):
        self.assertFalse(is_slidey(1123))

    def test_5(self):
        self.assertFalse(is_slidey(1357))

    def test_6(self):
        self.assertTrue(is_slidey(1))

    def test_7(self):
        self.assertTrue(is_slidey(0))

    def test_8(self):
        self.assertFalse(is_slidey(13578987))

    def test_9(self):
        self.assertTrue(is_slidey(232323232))

    def test_10(self):
        self.assertFalse(is_slidey(2323232322))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Slidey Numbers](https://edabit.com/challenge/od6i73gJxc6xGFzsz)
