# Challenge 388 - Making a Sandwich

Given a list of ingredients and a flavor, create a function that returns the list, but with the elements `"bread"` around the selected ingredient.

## Examples
```python
make_sandwich(["tuna", "ham", "tomato"], "ham") ➞ ["tuna", "bread", "ham", "bread", "tomato"]

make_sandwich(["cheese", "lettuce"], "cheese") ➞ ["bread", "cheese", "bread", "lettuce"]

make_sandwich(["ham", "ham"], "ham") ➞ ["bread", "ham", "bread", "bread", "ham", "bread"]
```
## Notes

- You will always get valid inputs.
- Make two separate sandwiches if two of the same elements are next to each other

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def make_sandwich(ingredients: list[str], flavor: str) -> list[str]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(
            make_sandwich(["t", "h", "t"], "h"), ["t", "bread", "h", "bread", "t"]
        )

    def test_2(self):
        self.assertListEqual(
            make_sandwich(["c", "l"], "c"), ["bread", "c", "bread", "l"]
        )

    def test_3(self):
        self.assertListEqual(
            make_sandwich(["h", "h"], "h"),
            ["bread", "h", "bread", "bread", "h", "bread"],
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Making a Sandwich](https://edabit.com/challenge/cGaTqHsPfR5H6YBuj)
