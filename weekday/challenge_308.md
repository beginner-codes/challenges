# Challenge 308 - Converting Dictionaries to Lists

Write a function that converts a dictionary into a list, where each element represents a key-value pair in the form of a list. Sort the list alphabetically by key.

## Examples
```python
to_list({ "a": 1, "b": 2 }) ➞ [["a", 1], ["b", 2]]

to_list({ "shrimp": 15, "tots": 12 }) ➞ [["shrimp", 15], ["tots", 12]]

to_list({}) ➞ []
```
## Notes

- Return an empty list if the dictionary is empty.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from typing import Union
import unittest


def to_list(dct: dict[str, int]) -> list[list[Union[str, int]]]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(to_list({"a": 1, "b": 2}), [["a", 1], ["b", 2]])

    def test_2(self):
        self.assertListEqual(
            to_list({"foo": 33, "bar": 45, "baz": 67}),
            [["bar", 45], ["baz", 67], ["foo", 33]],
        )

    def test_3(self):
        self.assertListEqual(
            to_list({"shrimp": 15, "tots": 12}), [["shrimp", 15], ["tots", 12]]
        )

    def test_4(self):
        self.assertListEqual(to_list({}), [])


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Converting Dictionaries to Lists](https://edabit.com/challenge/PgsQAdNvsEAkese8X)
