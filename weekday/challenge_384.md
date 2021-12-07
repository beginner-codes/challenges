# Challenge 384 - Rock, Paper, Scissors

Create a function which takes two strings as arguments and returns a string stating the winner in a game of Rock, Paper, Scissors.

Each argument will contain a single string: `"Rock"`, `"Paper"`, or `"Scissors"`. Return the winner according to the following rules:

- Rock beats Scissors
- Scissors beats Paper
- Paper beats Rock

If player 1 wins, return the string `"The winner is p1"`. If player 2 wins, return the string `"The winner is p2"` and if player 1 and player 2 are the same, return `"It's a draw"`.

## Examples
```python
rps("Rock", "Paper") ➞ "The winner is p2"

rps("Scissors", "Paper") ➞ "The winner is p1"

rps("Paper", "Paper") ➞ "It's a draw"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def rps(player_1: str, player_2: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(rps("Rock", "Paper"), "The winner is p2")

    def test_2(self):
        self.assertEqual(rps("Scissors", "Rock"), "The winner is p2")

    def test_3(self):
        self.assertEqual(rps("Scissors", "Paper"), "The winner is p1")

    def test_4(self):
        self.assertEqual(rps("Paper", "Rock"), "The winner is p1")

    def test_5(self):
        self.assertEqual(rps("Paper", "Paper"), "It's a draw")

    def test_6(self):
        self.assertEqual(rps("Rock", "Rock"), "It's a draw")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Rock, Paper, Scissors](https://edabit.com/challenge/sfqudQHQ3HPpd7dZb)
