# Challenge 401 - Split Item Codes

You have a list of item codes with the following format: `"[letters][digits]"`

Create a function that splits these strings into their alphabetic and numeric parts.

## Examples
```python
split_code("TEWA8392") ➞ ["TEWA", 8392]

split_code("MMU778") ➞ ["MMU", 778]

split_code("SRPE5532") ➞ ["SRPE", 5532]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def split_code(code: str) -> list[str, int]:
    return ["", 0]  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(split_code("TEWA8392"), ["TEWA", 8392])

    def test_2(self):
        self.assertListEqual(split_code("MMU778"), ["MMU", 778])

    def test_3(self):
        self.assertListEqual(split_code("SRPE5532"), ["SRPE", 5532])

    def test_4(self):
        self.assertListEqual(split_code("SKU8977"), ["SKU", 8977])

    def test_5(self):
        self.assertListEqual(split_code("MCI5589"), ["MCI", 5589])

    def test_6(self):
        self.assertListEqual(split_code("WIEB3921"), ["WIEB", 3921])


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Split Item Codes](https://edabit.com/challenge/CvChvza6kwweMjNRr)
