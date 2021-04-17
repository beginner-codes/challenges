# Challenge 227 - Connect Four

Take a look at wiki description of Connect Four game: https://en.wikipedia.org/wiki/Connect_Four

The grid is 6 rows by 7 columns, the columns being named A to G.

You will receive a list of strings showing the order of the pieces which were dropped into the columns:
```python
pieces_position_list = ["A_Red",
                        "B_Yellow",
                        "A_Red",
                        "B_Yellow",
                        "A_Red",
                        "B_Yellow",
                        "G_Red",
                        "B_Yellow"]
```
The list may contain up to 42 moves and shows the order the players are playing.

The first player who connects four items of the same color is the winner.

You should return `"Yellow"`, `"Red"` or `"Draw"` accordingly.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def who_is_winner(plays: list[str]) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(who_is_winner([
            "C_Yellow", "E_Red", "G_Yellow", "B_Red", "D_Yellow", "B_Red", "B_Yellow", "G_Red", "C_Yellow", "C_Red",
            "D_Yellow", "F_Red", "E_Yellow", "A_Red", "A_Yellow", "G_Red", "A_Yellow", "F_Red", "F_Yellow", "D_Red",
            "B_Yellow", "E_Red", "D_Yellow", "A_Red", "G_Yellow", "D_Red", "D_Yellow", "C_Red"
        ]), "Yellow")

    def test_2(self):
        self.assertEqual(who_is_winner([
            "C_Yellow", "B_Red", "B_Yellow", "E_Red", "D_Yellow", "G_Red", "B_Yellow", "G_Red", "E_Yellow", "A_Red",
            "G_Yellow", "C_Red", "A_Yellow", "A_Red", "D_Yellow", "B_Red", "G_Yellow", "A_Red", "F_Yellow", "B_Red",
            "D_Yellow", "A_Red", "F_Yellow", "F_Red", "B_Yellow", "F_Red", "F_Yellow", "G_Red", "A_Yellow", "F_Red",
            "C_Yellow", "C_Red", "G_Yellow", "C_Red", "D_Yellow", "D_Red", "E_Yellow", "D_Red", "E_Yellow", "C_Red",
            "E_Yellow", "E_Red"
        ]), "Yellow")

    def test_3(self):
        self.assertEqual(who_is_winner([
            "F_Yellow", "G_Red", "D_Yellow", "C_Red", "A_Yellow", "A_Red", "E_Yellow", "D_Red", "D_Yellow", "F_Red",
            "B_Yellow", "E_Red", "C_Yellow", "D_Red", "F_Yellow", "D_Red", "D_Yellow", "F_Red", "G_Yellow", "C_Red",
            "F_Yellow", "E_Red", "A_Yellow", "A_Red", "C_Yellow", "B_Red", "E_Yellow", "C_Red", "E_Yellow", "G_Red",
            "A_Yellow", "A_Red", "G_Yellow", "C_Red", "B_Yellow", "E_Red", "F_Yellow", "G_Red", "G_Yellow", "B_Red",
            "B_Yellow", "B_Red"
        ]), "Red")

    def test_4(self):
        self.assertEqual(who_is_winner([
            "A_Yellow", "B_Red", "B_Yellow", "C_Red", "G_Yellow", "C_Red", "C_Yellow", "D_Red", "G_Yellow", "D_Red",
            "G_Yellow", "D_Red", "F_Yellow", "E_Red", "D_Yellow"
        ]), "Red")

    def test_5(self):
        self.assertEqual(who_is_winner([
            "A_Red", "B_Yellow", "A_Red", "B_Yellow", "A_Red", "B_Yellow", "G_Red", "B_Yellow"
        ]), "Yellow")

    def test_6(self):
        self.assertEqual(who_is_winner([
            "A_Red", "B_Yellow", "A_Red", "E_Yellow", "F_Red", "G_Yellow", "A_Red", "G_Yellow"
        ]), "Draw");


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on CodeWars: [Connect Four](https://www.codewars.com/kata/56882731514ec3ec3d000009/train/python)
