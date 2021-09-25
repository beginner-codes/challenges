# Challenge 342 - Tic Tac Toe

Given a 3x3 matrix of a completed tic-tac-toe game, create a function that returns whether the game is a win for `"X"`, `"O"`, or a `"Draw"`, where `"X"` and `"O"` represent themselves on the matrix, and `"E"` represents an empty spot.

## Examples
```python
tic_tac_toe([
  ["X", "O", "X"],
  ["O", "X",  "O"],
  ["O", "X",  "X"]
]) ➞ "X"

tic_tac_toe([
  ["O", "O", "O"],
  ["O", "X", "X"],
  ["E", "X", "X"]
]) ➞ "O"

tic_tac_toe([
  ["X", "X", "O"],
  ["O", "O", "X"],
  ["X", "X", "O"]
]) ➞ "Draw"
```
## Notes

- Make sure that if `O` wins, you return the letter `"O"` and not the integer `0` (zero) and if it's a draw, make sure you return the capitalised word `"Draw"`. If you return `"X"` or `"O"`, make sure they're capitalised too.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def tic_tac_toe(board: list[list[str]]) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(
            tic_tac_toe([["X", "O", "X"], ["O", "X", "O"], ["O", "X", "X"]]), "X"
        )

    def test_2(self):
        self.assertEqual(
            tic_tac_toe([["O", "O", "O"], ["O", "X", "X"], ["E", "X", "X"]]), "O"
        )

    def test_3(self):
        self.assertEqual(
            tic_tac_toe([["X", "X", "O"], ["O", "O", "X"], ["X", "X", "O"]]), "Draw"
        )

    def test_4(self):
        self.assertEqual(
            tic_tac_toe([["X", "O", "O"], ["X", "O", "O"], ["X", "X", "X"]]), "X"
        )

    def test_5(self):
        self.assertEqual(
            tic_tac_toe([["X", "X", "O"], ["O", "O", "X"], ["X", "X", "O"]]), "Draw"
        )

    def test_6(self):
        self.assertEqual(
            tic_tac_toe([["X", "O", "X"], ["O", "X", "O"], ["E", "E", "X"]]), "X"
        )

    def test_7(self):
        self.assertEqual(
            tic_tac_toe([["X", "O", "E"], ["X", "O", "E"], ["E", "O", "X"]]), "O"
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Tic Tac Toe](https://edabit.com/challenge/A8gEGRXqMwRWQJvBf)
