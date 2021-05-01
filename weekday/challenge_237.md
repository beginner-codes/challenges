# Challenge 237 - Mastermind

The classic game of Mastermind is played on a tray on which the Mastermind conceals a code and the Guesser has 10 tries to guess it. The code is a sequence of 4 or more)zpegs of different colors. Each guess is a corresponding sequence of 4 or more pegs of different colors. A guess is "correct" when the color of every peg in the guess exactly matches the corresponding peg in the Mastermind's code.

After each guess by the Guesser, the Mastermind will give a score comprising black & white pegs, not arranged in any order:

- Black peg == guess peg matches the color of a code peg in the same position.
- White peg == guess peg matches the color of a code peg in another position.

Create a function that takes two strings, the mastermind's code and the guess as arguments, and returns the score in a dictionary (number of black pegs and number of white pegs).

- The code and guess are strings of numeric digits
- The color of the pegs are represented by numeric digits
- no "peg" may be double-scored

## Examples
```python
guess_score("1423", "5678") ➞ {"black": 0, "white": 0}

guess_score("1423", "2222") ➞ {"black": 1, "white": 0}

guess_score("1423", "1234") ➞ {"black": 1, "white": 3}

guess_score("1423", "2211") ➞ {"black": 0, "white": 2}
```
## Notes

- The code and guess sequences will have the same length.
- The "pegs" consists of only digits from 0-9.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def guess_score(masterminds_code: str, guess: str) -> dict[str, int]:
    return {}  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(guess_score("1423", "5678"), {"black": 0, "white": 0})

    def test_2(self):
        self.assertEqual(guess_score("1423", "2222"), {"black": 1, "white": 0})

    def test_3(self):
        self.assertEqual(guess_score("1423", "1234"), {"black": 1, "white": 3})

    def test_4(self):
        self.assertEqual(guess_score("1423", "2211"), {"black": 0, "white": 2})

    def test_5(self):
        self.assertEqual(guess_score("2928", "7722"), {"black": 1, "white": 1})

    def test_6(self):
        self.assertEqual(guess_score("4845", "6446"), {"black": 1, "white": 1})


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Mastermind](https://edabit.com/challenge/2iibnCci6G42f8Mjr)
