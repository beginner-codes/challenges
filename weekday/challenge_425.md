# Challenge 425 - Names, Ages and Occupations

Write a function that maps a string into a dictionary of name, string, and occupation pairs.

## Examples
```python
organize("Jameel Saeb, 15, CEO of facebook") ➞ {
  "name": "Jameel Saeb",
  "age": 15,
  "occupation": "CEO of facebook"
}

organize("John Mayer, 41, Singer") ➞ {
  "name": "John Mayer",
  "age": 41,
  "occupation": "Singer"
}

organize("") ➞ {}
```
## Notes

- Return an empty dictionary if given an empty string.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from typing import TypedDict
import unittest


class InfoDict(TypedDict):
    age: int
    name: str
    occupation: str


def organize(information: str) -> InfoDict:
    return {}  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(
            organize("Jameel Saeb, 15, CEO of facebook"),
            {"name": "Jameel Saeb", "age": 15, "occupation": "CEO of facebook"},
        )

    def test_2(self):
        self.assertEqual(
            organize("John Mayer, 41, Singer"),
            {"name": "John Mayer", "age": 41, "occupation": "Singer"},
        )

    def test_3(self):
        self.assertEqual(
            organize("Emily Blunt, 36, Actor"),
            {"name": "Emily Blunt", "age": 36, "occupation": "Actor"},
        )

    def test_4(self):
        self.assertEqual(
            organize("Conan O'Brien, 56, Talk Show Host"),
            {"name": "Conan O'Brien", "age": 56, "occupation": "Talk Show Host"},
        )

    def test_5(self):
        self.assertEqual(
            organize("Georg bullock, 31, Brother of an actor"),
            {"name": "Georg bullock", "age": 31, "occupation": "Brother of an actor"},
        )

    def test_6(self):
        self.assertEqual(organize(""), {})


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Names, Ages and Occupations](https://edabit.com/challenge/7nfSdzzpvTta8hhNe)
