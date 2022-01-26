# Challenge 402 - Height of the Tallest Building

Given a list of strings (depicting a skyline of several buildings), return in meters the height of the tallest building. Each line in the list represents 20 meters.

## Examples
```python
tallest_building_height([
  "            ##",
  "            ##",
  "            ##",
  "###   ###   ##",
  "###   ###   ###",
  "###   ###   ###",
  "###   ###   ###"
]) ➞ "140m"

# Tallest building is 7 characters
# 7 x 20m = 140m

tallest_building_height([
  "               ",
  "               ",
  "               ",
  "       #    ###",
  "      # #   ###",
  "###   ###   ###",
  "###   ###   ###"
]) ➞ "80m"

# Tallest building is 4 characters
# 4 x 20m = 80m

tallest_building_height([
  "                              ",
  "                         ###  ",
  "                         ###  ",
  "###                    #####  ",
  "###      #             #####  ",
  "###     ###            #####  ",
  "######  ###            #######",
  "######  ######  ###    #######",
  "###################    #######",
  "###############################",
  "###############################"
]) ➞ "200m"

# Tallest building is 10 characters
# 10 x 20m = 200m
```
## Notes

- There may be some open sky above buildings (can't just find the length of the list).

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
