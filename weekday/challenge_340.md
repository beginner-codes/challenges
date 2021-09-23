# Challenge 340 - Baseball Batting Average

A baseball player's batting average is calculated by the following formula:
```
BA = (number of hits) / (number of official at-bats)
```
Batting averages are always expressed rounded to the nearest thousandth with no leading zero. The top 3 MLB batting averages of all-time are:

- Ty Cobb .366
- Rogers Hornsby .358
- Shoeless Joe Jackson .356

Write a functino that takes a list that represents a season of games. Each list item indicates a player's `[hits, official at bats]` per game. Return a string with the player's seasonal batting average rounded to the nearest thousandth.

## Examples
```python
batting_avg([[0, 0], [1, 3], [2, 2], [0, 4], [1, 5]]) ➞ ".286"

batting_avg([[2, 5], [2, 3], [0, 3], [1, 5], [2, 4]]) ➞ ".350"

batting_avg([[2, 3], [1, 5], [2, 4], [1, 5], [0, 5]]) ➞ ".273"
```
## Notes

- The number of hits will not exceed the number of official at-bats.
- The list includes official at-bats only. No other plate-appearances (walks, hit-by-pitches, sacrifices, etc.) are included in the list.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def batting_avg(numbers: list[int]) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(batting_avg([[0, 0], [1, 3], [2, 2], [0, 4], [1, 5],]), ".286")

    def test_2(self):
        self.assertEqual(batting_avg([[2, 5], [2, 3], [0, 3], [1, 5], [2, 4],]), ".350")

    def test_3(self):
        self.assertEqual(batting_avg([[2, 3], [1, 5], [2, 4], [1, 5], [0, 5],]), ".273")

    def test_4(self):
        self.assertEqual(batting_avg([[1, 4], [0, 5], [4, 4], [1, 5], [0, 5],]), ".261")

    def test_5(self):
        self.assertEqual(batting_avg([[3, 3], [0, 5], [0, 4], [3, 5], [1, 5],]), ".318")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Baseball Batting Average](https://edabit.com/challenge/R4D59C9CQbJvqWaKd)
