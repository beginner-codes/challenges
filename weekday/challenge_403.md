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


def golf_score(par: list[int], result: list[str]) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(
            golf_score(
                [4, 4, 4, 4, 5, 3, 3, 4, 3, 5, 4, 4, 3, 4, 5, 4, 4, 5],
                ["double-bogey", "par", "par", "double-bogey", "eagle", "par", "bogey", "birdie", "birdie", "bogey", "par", "birdie", "par", "par", "par", "par", "bogey", "par"],
            ),
            74,
        )

    def test_2(self):
        self.assertEqual(
            golf_score(
                [5, 4, 4, 4, 4, 4, 5, 4, 3, 3, 4, 5, 3, 4, 4, 3, 5, 4],
                ["par", "bogey", "birdie", "bogey", "par", "birdie", "par", "bogey", "eagle", "par", "par", "birdie", "par", "eagle", "double-bogey", "birdie", "par", "birdie"],
            ),
            68,
        )

    def test_3(self):
        self.assertEqual(
            golf_score(
                [4, 3, 4, 4, 5, 4, 5, 4, 4, 4, 3, 5, 4, 4, 3, 4, 3, 5],
                ["bogey", "par", "birdie", "par", "par", "birdie", "bogey", "par", "par", "double-bogey", "par", "double-bogey", "par", "eagle", "par", "par", "par", "par"],
            ),
            74,
        )

    def test_4(self):
        self.assertEqual(
            golf_score(
                [4, 5, 4, 4, 4, 5, 5, 3, 4, 5, 4, 3, 4, 3, 3, 4, 4, 4],
                ["par", "par", "eagle", "bogey", "birdie", "par", "par", "par", "birdie", "eagle", "bogey", "bogey", "par", "par", "par", "par", "birdie", "bogey"],
            ),
            69,
        )

    def test_5(self):
        self.assertEqual(
            golf_score(
                [5, 5, 3, 5, 4, 4, 3, 4, 4, 4, 3, 3, 4, 4, 4, 5, 4, 4],
                ["birdie", "par", "par", "par", "bogey", "bogey", "bogey", "double-bogey", "par", "par", "par", "par", "eagle", "par", "double-bogey", "par", "birdie", "par"],
            ),
            75,
        )

if __name__ == "__main__":
    unittest.main()

```
## Credits

Found on Edabit: [What's My Golf Score?](https://edabit.com/challenge/wZzZ9NtugwsnQEQeM)
