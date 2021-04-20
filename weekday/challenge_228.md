# Challenge 228 - Add Suffix

Write a function that returns a lambda expression, which transforms its input by adding a particular suffix at the end.

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
    return lambda x: x  # Put your code here!!!


class Tests(unittest.TestCase):
    add_ing = add_suffix("ing")
    add_less = add_suffix("less")
    add_ly = add_suffix("ly")

    def test_1(self):
        self.assertEqual(self.add_ly("hopeless"), "hopelessly")

    def test_2(self):
        self.assertEqual(self.add_ly("total"), "totally")

    def test_3(self):
        self.assertEqual(self.add_less("fear"), "fearless")

    def test_4(self):
        self.assertEqual(self.add_less("ruth"), "ruthless")

    def test_5(self):
        self.assertEqual(self.add_ing("cheer"), "cheering")

    def test_6(self):
        self.assertEqual(self.add_ing("book"), "booking")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [All About Lambda Expressions: Adding Suffixes](https://edabit.com/challenge/nn7JKRBfq8iDcX8ZB)
