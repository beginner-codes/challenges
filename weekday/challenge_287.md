# Challenge 287 - Infection of the Ones

Write a function that replaces every row and column that contains at least a single 1 into a row/column that is filled entirely with 1s.

## Examples
```python
ones_infection(
    [
        [0, 0, 1],
        [0, 0, 0],
        [0, 0, 0]
    ]
) ➞ [
    [1, 1, 1],
    [0, 0, 1],
    [0, 0, 1]
]

ones_infection(
    [
        [1, 0, 1, 0],
        [0, 1, 0, 0],
        [0, 0, 0, 0]
    ]
) ➞ [
    [1, 1, 1, 1],
    [1, 1, 1, 1],
    [1, 1, 1, 0]
]

ones_infection(
    [
        [0, 1, 0, 1],
        [0, 0, 0, 0],
        [0, 1, 0, 0]
    ]
) ➞ [
    [1, 1, 1, 1],
    [0, 1, 0, 1],
    [1, 1, 1, 1]
]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def ones_infection(string: list[list[int]]) -> list[list[int]]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(
            ones_infection([[0, 0, 1], [0, 0, 0], [0, 0, 0]]),
            [[1, 1, 1], [0, 0, 1], [0, 0, 1]],
        )

    def test_2(self):
        self.assertListEqual(
            ones_infection([[1, 0, 1, 0], [0, 1, 0, 0], [0, 0, 0, 0]]),
            [[1, 1, 1, 1], [1, 1, 1, 1], [1, 1, 1, 0]],
        )

    def test_3(self):
        self.assertListEqual(
            ones_infection([[0, 1, 0, 1], [0, 0, 0, 0], [0, 1, 0, 0]]),
            [[1, 1, 1, 1], [0, 1, 0, 1], [1, 1, 1, 1]],
        )

    def test_4(self):
        self.assertListEqual(
            ones_infection([[0, 1, 0, 1, 0], [0, 0, 0, 0, 0], [0, 1, 1, 1, 0]]),
            [[1, 1, 1, 1, 1], [0, 1, 1, 1, 0], [1, 1, 1, 1, 1]],
        )

    def test_5(self):
        self.assertListEqual(
            ones_infection([[1, 0, 1, 0], [0, 0, 0, 0], [0, 0, 0, 0]]),
            [[1, 1, 1, 1], [1, 0, 1, 0], [1, 0, 1, 0]],
        )

    def test_6(self):
        self.assertListEqual(
            ones_infection([[0, 0, 0, 1], [0, 0, 0, 0], [0, 0, 0, 0]]),
            [[1, 1, 1, 1], [0, 0, 0, 1], [0, 0, 0, 1]],
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Infection of the Ones](https://edabit.com/challenge/tY5fmSbk85N8digXQ)
