# Challenge 246 - Convert to Number

You prepare a list to send to the insurance company. As you finish, you notice you misformatted it. Given a dictionary with at least one key/value pair, convert all the values to numbers.

## Examples
```python
convert_to_number({ "piano": "200" }) ➞ { "piano": 200 }

convert_to_number({ "piano": "200", "tv": "300" }) ➞ { "piano": 200, "tv": 300 }

convert_to_number({ "piano": "200", "tv": "300", "stereo": "400" }) ➞ { "piano": 200, "tv": 300, "stereo": 400 }
```
## Notes

- You will only be tested for numbers (ints), not strings or floats.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from typing import Any
import unittest


def convert_to_number(inventory: dict[str, Any]) -> dict[str, int]:
    return {}  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(
            convert_to_number({"piano": "200", "tv": "300", "stereo": "400"}),
            {"piano": 200, "tv": 300, "stereo": 400},
        )

    def test_2(self):
        self.assertEqual(
            convert_to_number({"piano": "200", "tv": "300"}), {"piano": 200, "tv": 300}
        )

    def test_3(self):
        self.assertEqual(convert_to_number({"piano": "200"}), {"piano": 200})

    def test_4(self):
        self.assertEqual(
            convert_to_number(
                {
                    "one": "1",
                    "two": "2",
                    "three": "3",
                    "four": "4",
                    "five": "5",
                    "six": "6",
                    "seven": "7",
                    "eight": "8",
                }
            ),
            {
                "one": 1,
                "two": 2,
                "three": 3,
                "four": 4,
                "five": 5,
                "six": 6,
                "seven": 7,
                "eight": 8,
            },
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Burglary Series (06): Convert to Number](https://edabit.com/challenge/R7d5JE7NQCSnajuni)
