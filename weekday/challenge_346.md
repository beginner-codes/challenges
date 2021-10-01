# Challenge 346 - Back and Forth

In a board game, a player may pick up a card with several left or right facing arrows, with the number of arrows indicating the number of tiles to move. The player should move either left or right, depending on the arrow's direction.

Given a list of the arrows contained on a player's cards, create a function that returns a singular string of arrowheads that are equivalent to all of the arrowheads.

_Worked Example_
```python
calculate_arrowhead([">>", "<<", "<<<"]) ➞ "<<<"

# >> means to move 2 places right
# << means to move 2 places left (cancelling out >>)
# <<< means to move a further 3 places left
# overall, the movement can be written as <<<
```
## Examples
```python
calculate_arrowhead([">>>>", "<", "<", "<"]) ➞ ">"

calculate_arrowhead([">", "<", ">>", "<", "<<<"]) ➞ "<<"

calculate_arrowhead([">>>", "<<<"]) ➞ ""
```
## Notes

- Return an empty string if all the arrowheads cancel out.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def calculate_arrowhead(cards: list[str]) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(calculate_arrowhead([">>>>", "<", "<", "<"]), ">")

    def test_2(self):
        self.assertEqual(calculate_arrowhead([">", "<", ">>", "<", "<<<"]), "<<")

    def test_3(self):
        self.assertEqual(calculate_arrowhead([">>>", "<<<"]), "")

    def test_4(self):
        self.assertEqual(calculate_arrowhead([">>", "<<", "<<<"]), "<<<")

    def test_5(self):
        self.assertEqual(
            calculate_arrowhead(
                [">", ">>>>>", ">>>>", ">>>>>>>", ">>>>>>>>", ">>>>", ">>>>>>>>"]
            ),
            ">>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>",
        )

    def test_6(self):
        self.assertEqual(
            calculate_arrowhead(
                ["<", ">>>>>>", "<<<<<<<<", "<<<<<<<<<<", ">>>>>>>", ">>>"]
            ),
            "<<<",
        )

    def test_7(self):
        self.assertEqual(calculate_arrowhead(["<<<<", ">>>>>"]), ">")

    def test_8(self):
        self.assertEqual(
            calculate_arrowhead(
                ["<<<<<<<<<", "<<<<", ">>>", ">>>>>>>>", ">>>>>>>", "<<<<<"]
            ),
            "",
        )

    def test_9(self):
        self.assertEqual(
            calculate_arrowhead([">>>>>>>>>>", "<<", ">>>>>>>>>>"]),
            ">>>>>>>>>>>>>>>>>>",
        )

    def test_10(self):
        self.assertEqual(
            calculate_arrowhead([">", "<<<", ">>>>>>>>>>", ">>>>>"]), ">>>>>>>>>>>>>"
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Back and Forth](https://edabit.com/challenge/mhcjnns2WWiHWexP7)
