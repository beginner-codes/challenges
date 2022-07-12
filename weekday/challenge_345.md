# Challenge 345 - Peeling off the Outer Layers

Given a list of lists, create a function that returns a new list of lists containing every element, except for the outer elements.

## Examples
```python
peel_layer_off([
  [1, 2, 3, 4, 5],
  [6, 7, 8, 9, 10],
  [11, 12, 13, 14, 15],
  [16, 17, 18, 19, 20],
  [21, 22, 23, 24, 25],
  [26, 27, 28, 29, 30],
  [31, 32, 33, 34, 35]
]) ➞ [
  [7, 8, 9],
  [12, 13, 14],
  [17, 18, 19],
  [22, 23, 24],
  [27, 28, 29]
]

peel_layer_off([
  [True, False, True],
  [False, False, True],
  [True, True, True]
]) ➞ [[False]]

peel_layer_off([
  ["hello", "world"],
  ["hello", "world"]
]) ➞ []
```
## Notes

- The 2D grid is always a rectangular/square shape.
- Always return some form of nested list, unless there are no elements. In that case, return an empty list.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from typing import TypeVar
import unittest


Item = TypeVar("Item")


def peel_layer_off(unpeeled: list[list[Item]]) -> list[list[Item]]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(
            peel_layer_off(
                [
                    ["a", "b", "c", "d"],
                    ["e", "f", "g", "h"],
                    ["i", "j", "k", "l"],
                    ["m", "n", "o", "p"],
                ]
            ),
            [["f", "g"], ["j", "k"]],
        )

    def test_2(self):
        self.assertListEqual(
            peel_layer_off(
                [
                    [1, 2, 3, 4, 5],
                    [6, 7, 8, 9, 10],
                    [11, 12, 13, 14, 15],
                    [16, 17, 18, 19, 20],
                    [21, 22, 23, 24, 25],
                    [26, 27, 28, 29, 30],
                    [31, 32, 33, 34, 35],
                ]
            ),
            [[7, 8, 9], [12, 13, 14], [17, 18, 19], [22, 23, 24], [27, 28, 29],],
        )

    def test_3(self):
        self.assertListEqual(
            peel_layer_off(
                [[True, False, True], [False, False, True], [True, True, True]]
            ),
            [[False]],
        )

    def test_4(self):
        self.assertListEqual(
            peel_layer_off([["hello", "world"], ["hello", "world"]]), []
        )

    def test_5(self):
        self.assertListEqual(
            peel_layer_off(
                [
                    [True, False, True, 1, 2, 3, 4],
                    [False, False, True, 5, 6, 7, 8],
                    [True, True, True, 9, 10, 11, 12],
                ]
            ),
            [[False, True, 5, 6, 7]],
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Peeling off the Outer Layers](https://edabit.com/challenge/EWgdCtSDmRqJPrzoz)
