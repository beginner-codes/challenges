# Challenge 375 - Splitting Objects Inside a List

You bought a few bunches of fruit over the weekend. Create a function that splits a bunch into singular objects inside a list.

## Examples
```python
split_bunches([
  { "name": "grapes", "quantity": 2 }
]) ➞ [
  { "name": "grapes", "quantity": 1 },
  { "name": "grapes", "quantity": 1 }
]


split_bunches([
  { "name": "currants", "quantity": 1 },
  { "name": "grapes", "quantity": 2 },
  { "name": "bananas", "quantity": 2 }
]) ➞ [
  { "name": "currants", "quantity": 1},
  { "name": "grapes", "quantity": 1 },
  { "name": "grapes", "quantity": 1 },
  { "name": "bananas", "quantity": 1 },
  { "name": "bananas", "quantity": 1 }
]
```
## Notes

- The input list will never be empty.
- Objects will always have a name and quantity over 0.
- The returned object should have each fruit in the same order as the original.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def split_bunches(bunches: list[dict[str, str | int]]) -> list[dict[str, str | int]]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(
            split_bunches([{"name": "bananas", "quantity": 1}]),
            [{"name": "bananas", "quantity": 1}],
        )

    def test_2(self):
        self.assertListEqual(
            split_bunches(
                [{"name": "bananas", "quantity": 2}, {"name": "grapes", "quantity": 2}]
            ),
            [
                {"name": "bananas", "quantity": 1},
                {"name": "bananas", "quantity": 1},
                {"name": "grapes", "quantity": 1},
                {"name": "grapes", "quantity": 1},
            ],
        )

    def test_3(self):
        self.assertListEqual(
            split_bunches(
                [
                    {"name": "cherry tomatoes", "quantity": 3},
                    {"name": "bananas", "quantity": 1},
                    {"name": "grapes", "quantity": 2},
                    {"name": "cherry tomatoes", "quantity": 3},
                ]
            ),
            [
                {"name": "cherry tomatoes", "quantity": 1},
                {"name": "cherry tomatoes", "quantity": 1},
                {"name": "cherry tomatoes", "quantity": 1},
                {"name": "bananas", "quantity": 1},
                {"name": "grapes", "quantity": 1},
                {"name": "grapes", "quantity": 1},
                {"name": "cherry tomatoes", "quantity": 1},
                {"name": "cherry tomatoes", "quantity": 1},
                {"name": "cherry tomatoes", "quantity": 1},
            ],
        )

    def test_4(self):
        self.assertListEqual(
            split_bunches(
                [
                    {"name": "currants", "quantity": 1},
                    {"name": "grapes", "quantity": 2},
                    {"name": "bananas", "quantity": 2},
                ]
            ),
            [
                {"name": "currants", "quantity": 1},
                {"name": "grapes", "quantity": 1},
                {"name": "grapes", "quantity": 1},
                {"name": "bananas", "quantity": 1},
                {"name": "bananas", "quantity": 1},
            ],
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: Splitting Objects Inside a List(https://edabit.com/challenge/zXACKeaEzLK9XwBwp)
