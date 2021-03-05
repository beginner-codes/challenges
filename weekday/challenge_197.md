# Challenge 197 - Can You Spare a Square?

Try to imagine a world in which you might have to stay home for 14 days at any given time. Do you have enough TP to make it through?

Although the number of squares per roll of TP varies significantly, we'll assume each roll has `500` sheets, and the average person uses `57` sheets per day.

Create a function that will receive a dictionary with two key/values:

- `"people"` — Number of people in the household.
- `"tp"` — Number of rolls.

Return a statement telling the user if they need to buy more TP!

## Examples
```python
tp_checker({ "people": 4, "tp": 1 }) ➞ "Your TP will only last 2 days, buy more!"

tp_checker({ "people": 3, "tp": 20 }) ➞ "Your TP will last 58 days, no need to panic!"

tp_checker({ "people": 4, "tp": 12 }) ➞ "Your TP will last 26 days, no need to panic!"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def tp_checker(home: dict[str:int]) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(
            tp_checker({"people": 4, "tp": 1}),
            "Your TP will only last 2 days, buy more!",
        )

    def test_2(self):
        self.assertEqual(
            tp_checker({"people": 2, "tp": 4}),
            "Your TP will last 17 days, no need to panic!",
        )

    def test_3(self):
        self.assertEqual(
            tp_checker({"people": 3, "tp": 20}),
            "Your TP will last 58 days, no need to panic!",
        )

    def test_4(self):
        self.assertEqual(
            tp_checker({"people": 4, "tp": 12}),
            "Your TP will last 26 days, no need to panic!",
        )

    def test_5(self):
        self.assertEqual(
            tp_checker({"people": 6, "tp": 8}),
            "Your TP will only last 11 days, buy more!",
        )

    def test_6(self):
        self.assertEqual(
            tp_checker({"people": 1, "tp": 1}),
            "Your TP will only last 8 days, buy more!",
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Can You Spare a Square?](https://edabit.com/challenge/joCBaJztZrdxi9HjR)
