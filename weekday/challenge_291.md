# Challenge 291 - Is It Gone?

Given a dictionary of the stolen items and a lowercase string that is the name of the pet (e.g. "rambo"), return:

- `"Rambo is gone..."` if the name is in the dictionary.
- `"Rambo is here!"` if the name is not in the dictionary.

*Note that the first letter of the name in the return statement is capitalized.*

## Examples
```python
items = {
  "tv": 30,
  "timmy": 20,
  "stereo": 50,
} ➞ "Timmy is gone..."
# Timmy is in the dictionary.


items = {
  "tv": 30,
  "stereo": 50,
} ➞ "Timmy is here!"
# Timmy is not in the  dictionary.


items = {} ➞ "Timmy is here!"
# Timmy is not in the dictionary.
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def find_it(stolen_items: dict[str, int], pets_name: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(find_it({}, "rambo"), "Rambo is here!")

    def test_2(self):
        self.assertEqual(find_it({}, "heman"), "Heman is here!")

    def test_3(self):
        self.assertEqual(
            find_it(
                {
                    "tv": 30,
                    "stereo": 50,
                },
                "rocky",
            ),
            "Rocky is here!",
        )

    def test_4(self):
        self.assertEqual(
            find_it(
                {
                    "tv": 30,
                    "stereo": 50,
                },
                "spiderman",
            ),
            "Spiderman is here!",
        )

    def test_5(self):
        self.assertEqual(
            find_it(
                {
                    "tv": 30,
                    "stereo": 50,
                    "julius": 100,
                },
                "julius",
            ),
            "Julius is gone...",
        )

    def test_6(self):
        self.assertEqual(
            find_it(
                {
                    "tv": 30,
                    "stereo": 50,
                    "batman": 200,
                },
                "batman",
            ),
            "Batman is gone...",
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Burglary Series (03): Is It Gone?](https://edabit.com/challenge/2wQPKcSipXmK4idwD)
