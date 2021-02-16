# Challenge 184 - Wash Your Hands :)

It takes 21 seconds to wash your hands and help prevent the spread of COVID-19.

Create a function that takes the number of times a person washes their hands per day and the number of months they follow this routine and calculates the duration in minutes and seconds that person spends washing their hands.

## Examples
```python
wash_hands(8, 7) ➞ "588 minutes and 0 seconds"

wash_hands(0, 0) ➞ "0 minutes and 0 seconds"

wash_hands(7, 9) ➞ "661 minutes and 30 seconds"
```
## Notes

- Consider a month has 30 days.
- Wash your hands.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```py
import unittest


def wash_hands(times_daily: int, total_months: int) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(wash_hands(8, 7), "588 minutes and 0 seconds")

    def test_2(self):
        self.assertEqual(wash_hands(20, 10), "2100 minutes and 0 seconds")

    def test_3(self):
        self.assertEqual(wash_hands(7, 9), "661 minutes and 30 seconds")

    def test_4(self):
        self.assertEqual(wash_hands(0, 2), "0 minutes and 0 seconds")

    def test_5(self):
        self.assertEqual(wash_hands(13, 3), "409 minutes and 30 seconds")

    def test_6(self):
        self.assertEqual(wash_hands(1, 1), "10 minutes and 30 seconds")

    def test_7(self):
        self.assertEqual(wash_hands(7, 0), "0 minutes and 0 seconds")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Wash Your Hands :)](https://edabit.com/challenge/7RPtGySfZLkEHB8ac)
