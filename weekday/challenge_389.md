# Challenge 389 - Are They the Same?

Create a function that takes three arguments (first dictionary, second dictionary, key). The function should do the following:

- Return `True` if both dictionaries have the same values for the key.
- If the dictionaries don't match, return the string `"Not the same"`, or the string `"One's empty"` if only one of the dictionaries contains the given key.

## Examples
```python
dict_first = { "sky": "temple", "horde": "orcs", "people": 12, "story": "fine", "sun": "bright" }
dict_second = { "people": 12, "sun": "star", "book": "bad" }

check(dict_first, dict_second, "horde") ➞ "One's empty"

check(dict_first, dict_second, "people") ➞ True

check(dict_first, dict_second, "sun") ➞ "Not the same"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from typing import Any
import unittest


def check(dict_a: dict[str, Any], dict_b: dict[str, Any], key: str) -> str | bool:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def setUp(self) -> None:
        self.dict_a = {
            "sky": "blue",
            "road": "broken",
            "sun": "star",
            "tree": "tall",
            "car": "noisy",
            "study": "hard",
            "price": 500,
        }
        self.dict_b = {
            "sun": "star",
            "book": "bad",
            "sky": "temple",
            "people": 12,
            "price": 500,
            "car": "auto",
            "study": "hard",
        }

    def test_1(self):
        self.assertEqual(check(self.dict_a, self.dict_b, "sky"), "Not the same")

    def test_2(self):
        self.assertEqual(check(self.dict_a, self.dict_b, "sun"), True)

    def test_3(self):
        self.assertEqual(check(self.dict_a, self.dict_b, "tree"), "One's empty")

    def test_4(self):
        self.assertEqual(check(self.dict_a, self.dict_b, "road"), "One's empty")

    def test_5(self):
        self.assertEqual(check(self.dict_a, self.dict_b, "car"), "Not the same")

    def test_6(self):
        self.assertEqual(check(self.dict_a, self.dict_b, "book"), "One's empty")

    def test_7(self):
        self.assertEqual(check(self.dict_a, self.dict_b, "study"), True)

    def test_8(self):
        self.assertEqual(check(self.dict_a, self.dict_b, "people"), "One's empty")

    def test_9(self):
        self.assertEqual(check(self.dict_a, self.dict_b, "price"), True)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Are They the Same?](https://edabit.com/challenge/fyyJRDHcTe9REs4Ni)
