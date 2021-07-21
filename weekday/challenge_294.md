# Challenge 294 - List Multiplier

Create a function that takes a list as an argument and returns a new nested list for each element in the original list. The nested list must be filled with the corresponding element (string or number) in the original list and each nested list has the same amount of elements as the original list.

## Examples
```python
multiply([4, 5]) ➞ [[4, 4], [5, 5]]

multiply(["*", "%", "$"]) ➞ [["*", "*", "*"], ["%", "%", "%"], ["$", "$", "$"]]

multiply(["A", "B", "C", "D", "E"]) ➞ [
    ["A", "A", "A", "A", "A"],
    ["B", "B", "B", "B", "B"],
    ["C", "C", "C", "C", "C"],
    ["D", "D", "D", "D", "D"],
    ["E", "E", "E", "E", "E"]
]
```
## Notes

- The given list contains numbers or strings.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from typing import Union
import unittest


def multiply(lst: list[Union[int, str]]) -> list[list[Union[int, str]]]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(
            multiply(["*", "%", "$"]),
            [["*", "*", "*"], ["%", "%", "%"], ["$", "$", "$"]],
        )

    def test_2(self):
        self.assertListEqual(multiply([4, 5]), [[4, 4], [5, 5]])

    def test_3(self):
        self.assertListEqual(
            multiply(["A", "B", "C", "D", "E"]),
            [
                ["A", "A", "A", "A", "A"],
                ["B", "B", "B", "B", "B"],
                ["C", "C", "C", "C", "C"],
                ["D", "D", "D", "D", "D"],
                ["E", "E", "E", "E", "E"],
            ],
        )

    def test_4(self):
        self.assertListEqual(multiply([1]), [[1]])


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [List Multiplier](https://edabit.com/challenge/8oNKM4osgxYyrFtGL)
