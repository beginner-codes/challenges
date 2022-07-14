# Challenge 301 - Match the Last Item

Create a function that takes a list of items and checks if the last item matches the rest of the list concatenated together.

## Examples
```python
match_last_item(["rsq", "6hi", "g", "rsq6hig"]) ➞ True
# The last item is the rest joined.

match_last_item([1, 1, 1, "11"]) ➞ False
# The last item should be "111".

match_last_item([8, "thunder", True, "8thunderTrue"]) ➞ True
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from typing import Any
import unittest


def match_last_item(items: list[Any]) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(match_last_item(["rsq", "6hi", "g", "rsq6hig"]))

    def test_2(self):
        self.assertFalse(match_last_item([0, 1, 2, 3, 4, 5, "12345"]))

    def test_3(self):
        self.assertFalse(match_last_item(["for", "mi", "da", "bel", "formidable"]))

    def test_4(self):
        self.assertTrue(match_last_item([8, "thunder", True, "8thunderTrue"]))

    def test_5(self):
        self.assertFalse(match_last_item([1, 1, 1, "11"]))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Match the Last Item](https://edabit.com/challenge/oGkwLhmpys95rjtQ2)
