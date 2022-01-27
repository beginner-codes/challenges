# Challenge 403 - What's My Golf Score?

A standard-sized golf course has 18 holes. Each hole is given a par, which is the expected number of strokes (hits) that a good player would use to complete a hole. Golf also uses different terms for a player being over/under par for a particular hole:

- `"eagle"` = 2 under par (-2)
- `"birdie"` = 1 under par (-1)
- `"bogey"` = 1 over par (+1)
- `"double-bogey"` = 2 over par (+2)

*Example scores:*

- `"birdie"` on a par 3 hole = 2
- `"eagle"` on a par 5 hole = 3
- `"par"` on a par 3 hole = 3
- `"bogey"` on a par 4 hole = 5

Given a list of pars for an 18-hole golf course, and another list containing the player result for each hole, return the total score for the round of golf.

## Example
```python
course = [4, 4, 5, 3, 4, 4, 3, 5, 5, 3, 5, 4, 4, 4, 4, 3, 4, 4]

result = ["eagle", "bogey", "par", "bogey", "double-bogey", "birdie", "bogey", "par", "birdie", "par", "par", "par", "par", "par", "bogey", "eagle", "bogey", "par"]

score = 2+5+5+4+6+3+4+5+4+3+5+4+4+4+5+1+5+4 = 73
```
## Notes

- For this challenge, there will be no holes-in-one, albatrosses (-3), or anything worse than a double-bogey.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def tallest_building_height(skyline: list[str]) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(
            tallest_building_height(
                [
                    "         ",
                    " ##      ",
                    " ##      ",
                    "###   ## ",
                    "###   ## ",
                    "###   ###",
                    "###   ###",
                ]
            ),
            "120m",
        )

    def test_2(self):
        self.assertEqual(
            tallest_building_height(
                [
                    "            ## ",
                    "            ## ",
                    "            ## ",
                    "###   ###   ## ",
                    "###   ###   ###",
                    "###   ###   ###",
                    "###   ###   ###",
                ]
            ),
            "140m",
        )

    def test_3(self):
        self.assertEqual(
            tallest_building_height(
                [
                    "               ",
                    "               ",
                    "               ",
                    "       #    ###",
                    "      # #   ###",
                    "###   ###   ###",
                    "###   ###   ###",
                ]
            ),
            "80m",
        )

    def test_4(self):
        self.assertEqual(
            tallest_building_height(
                [
                    "               ",
                    "               ",
                    "               ",
                    "               ",
                    "               ",
                    "###   ###   ###",
                    "###   ###   ###",
                ]
            ),
            "40m",
        )

    def test_5(self):
        self.assertEqual(
            tallest_building_height(
                [
                    "                   ",
                    " #                 ",
                    " #     #           ",
                    "###    #    ###    ",
                    "###   # #   ###   #",
                    "###   ###   ###   #",
                    "###   ###   ###   #",
                ]
            ),
            "120m",
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Height of the Tallest Building](https://edabit.com/challenge/LuBtaT9dwStbd7mnK)
