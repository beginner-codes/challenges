# Challenge 247 - The Fiscal Code

Given an dictionary containing the personal data of a person (name, surname, gender and date of birth) return the 11 code characters as a string following these steps:

__Generate 3 capital letters from the surname, if it has:__
- At least 3 consonants then the first three consonants are used. (Newman -> NWM).
- Less than 3 consonants then vowels will replace missing characters in the same order they appear (Fox -> FXO | Hope -> HPO).
- Less than three letters then "X" will take the third slot after the consonant and the vowel (Yu -> YUX).

__Generate 3 capital letters from the name, if it has:__
- Exactly 3 consonants then consonants are used in the order they appear (Matt -> MTT).
- More than 3 consonants then first, third and fourth consonant are used (Samantha -> SNT | Thomas -> TMS).
- Less than 3 consonants then vowels will replace missing characters in the same order they appear (Bob -> BBO | Paula -> PLA).
- Less than three letters then "X" will take the the third slot after the consonant and the vowel (Al -> LAX).

__Generate 2 numbers, 1 letter and 2 numbers from date of birth and "gender":__
- Take the last two digits of the year of birth (1985 -> 85).
- Generate a letter corresponding to the month of birth (January -> A | December -> T) using the table below
- For males take the day of birth adding one zero at the start if is less than 10 (any 9th day -> 09 | any 20th day -> 20).
- For females take the day of birth and sum 40 to it (any 9th day -> 49 | any 20th day -> 60).
    
Month Conversion Table:
```
Jan ➞ A
Feb ➞ B
Mar ➞ C
Apr ➞ D
May ➞ E
Jun ➞ H
Jul ➞ L
Aug ➞ M
Sep ➞ P
Oct ➞ R
Nov ➞ S
Dec ➞ T
```
## Examples
```python
fiscal_code({
  "name": "Matt",
  "surname": "Edabit",
  "gender": "M",
  "dob": "1/1/1900"
}) ➞ "DBTMTT00A01"

fiscal_code({
  "name": "Helen",
  "surname": "Yu",
  "gender": "F",
  "dob": "1/12/1950"
}) ➞ "YUXHLN50T41"

fiscal_code({
  "name": "Mickey",
  "surname": "Mouse",
  "gender": "M",
  "dob": "16/1/1928"
}) ➞ "MSOMKY28A16"
```
## Notes

- Code letters must be uppercase.
- Date of birth is given in D/M/YYYY format.
- Y is not a vowel.

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
