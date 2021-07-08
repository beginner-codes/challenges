# Challenge 285 - Count Letters in a Word Search

Create a function that counts the number of times a particular letter shows up in the word search.

## Examples
```python
letter_counter([
["D", "E", "Y", "H", "A", "D"],
["C", "B", "Z", "Y", "J", "K"],
["D", "B", "C", "A", "M", "N"],
["F", "G", "G", "R", "S", "R"],
["V", "X", "H", "A", "S", "S"]
], "D") ➞ 3

# "D" shows up 3 times: twice in the first row, once in the third row.

letter_counter([
["D", "E", "Y", "H", "A", "D"],
["C", "B", "Z", "Y", "J", "K"],
["D", "B", "C", "A", "M", "N"],
["F", "G", "G", "R", "S", "R"],
["V", "X", "H", "A", "S", "S"]
], "H") ➞ 2
```
## Notes

- You will always be given a 2 dimensional list

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def letter_counter(word_search: list[list[str]], letter: str) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(
            letter_counter([
                ["D", "E", "Y", "H", "A", "D"],
                ["C", "B", "Z", "Y", "J", "K"],
                ["D", "B", "C", "A", "M", "N"],
                ["F", "G", "G", "R", "S", "R"],
                ["V", "X", "H", "A", "S", "S"],
            ], "D"),
            3,
        )

    def test_2(self):
        self.assertEqual(
            letter_counter([
                ["D", "E", "Y", "H", "A", "D"],
                ["C", "B", "Z", "Y", "J", "K"],
                ["D", "B", "C", "A", "M", "N"],
                ["F", "G", "G", "R", "S", "R"],
                ["V", "X", "H", "A", "S", "S"],
            ], "H"),
            2,
        )

    def test_3(self):
        self.assertEqual(
            letter_counter([
                ["D", "E", "Y", "H", "A", "D"],
                ["C", "B", "Z", "Y", "J", "K"],
                ["D", "B", "C", "A", "M", "N"],
                ["F", "G", "G", "R", "S", "R"],
                ["V", "X", "H", "A", "S", "S"],
            ], "Z"),
            1,
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Count Letters in a Word Search](https://edabit.com/challenge/czwN5HPjG3kbrqkp3)
