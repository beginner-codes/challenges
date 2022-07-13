# Challenge 309 - Add Suffix

Write a function that returns a function, which transforms its input by adding a particular suffix to the end.

## Examples
```python
add_ly = add_suffix("ly")
add_ly("hopeless") ➞ "hopelessly"
add_ly("total") ➞ "totally"

add_less = add_suffix("less")
add_less("fear") ➞ "fearless"
add_less("ruth") ➞ "ruthless"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from typing import Callable
import unittest


def add_suffix(suffix: str) -> Callable[[str], str]:
    return str  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        add_ly = add_suffix("ly")
        self.assertEqual(add_ly("hopeless"), "hopelessly")

    def test_2(self):
        add_ly = add_suffix("ly")
        self.assertEqual(add_ly("total"), "totally")

    def test_3(self):
        add_less = add_suffix("less")
        self.assertEqual(add_less("fear"), "fearless")

    def test_4(self):
        add_less = add_suffix("less")
        self.assertEqual(add_less("ruth"), "ruthless")

    def test_5(self):
        add_ing = add_suffix("ing")
        self.assertEqual(add_ing("cheer"), "cheering")

    def test_6(self):
        add_ing = add_suffix("ing")
        self.assertEqual(add_ing("book"), "booking")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [All About Lambda Expressions: Adding Suffixes](https://edabit.com/challenge/nn7JKRBfq8iDcX8ZB)
