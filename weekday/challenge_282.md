# Challenge 282 - Incrementing Rows and Columns

Write a function that takes in three parameters: `rows`, `columns`, and `operations`, where:

- `rows` and `columns` are the number of rows and columns to initialize a zero matrix.
- `operations` is the list of incrementing operations (+1) to be performed.

And returns the resulting matrix after applying all the increment operations. Each increment operation will add 1 to the rows or columns specified in the incrementing list.

To illustrate:
```python
final(3, 3, ["2r", "2c", "1r", "0c"])

# Initialize a 3 x 3 matrix of zeroes.

[
  [0, 0, 0],
  [0, 0, 0],
  [0, 0, 0]
]

# Apply "2r" (increment index 2 row).

[
  [0, 0, 0],
  [0, 0, 0],
  [1, 1, 1]
]

# Apply "2c" (increment index 2 column).

[
  [0, 0, 1],
  [0, 0, 1],
  [1, 1, 2]
]

# Apply "1r" (increment index 1 row).

[
  [0, 0, 1],
  [1, 1, 2],
  [1, 1, 2]
]

# Apply "0c" (increment index 0 column).
# This is the result you should return.

[
  [1, 0, 1],
  [2, 1, 2],
  [2, 1, 2]
]
```
## Examples
```python
final(2, 2, ["0r", "0r", "0r", "1c"]) ➞ [
  [3, 4],
  [0, 1]
]

final(2, 2, ["0c"]) ➞ [
  [1, 0],
  [1, 0]
]

final(3, 3, ["1c", "2c", "2c", "3c", "3c", "3c"]) ➞ [
    [1, 2, 3],
    [1, 2, 3],
    [1, 2, 3]
]

final(3, 3, []) ➞ [
  [0, 0, 0],
  [0, 0, 0],
  [0, 0, 0]
]
```
## Notes

- The 2D matrix is 0-indexed.
- The matrix created will have at least one row and one column.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def final(rows: int, columns: int, operations: list[str]) -> list[list[int]]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(final(2, 2, ["0r", "0r", "0r", "1c"]), [[3, 4], [0, 1]])

    def test_2(self):
        self.assertListEqual(final(2, 2, ["0c"]), [[1, 0], [1, 0]])

    def test_3(self):
        self.assertListEqual(
            final(3, 3, ["0c", "1c", "1c", "2c", "2c", "2c"]),
            [[1, 2, 3], [1, 2, 3], [1, 2, 3]],
        )

    def test_4(self):
        self.assertListEqual(
            final(3, 3, ["2r", "2c", "1r", "0c"]), [[1, 0, 1], [2, 1, 2], [2, 1, 2]]
        )

    def test_5(self):
        self.assertListEqual(final(1, 1, []), [[0]])

    def test_6(self):
        self.assertListEqual(
            final(3, 3, ["0r", "2c", "1r", "2c", "1c", "1r", "1r"]),
            [[1, 2, 3], [3, 4, 5], [0, 1, 2]],
        )

    def test_7(self):
        self.assertListEqual(final(3, 3, []), [[0, 0, 0], [0, 0, 0], [0, 0, 0]])

    def test_8(self):
        self.assertListEqual(
            final(3, 4, ["1r", "1r", "1r", "3c", "3c", "3c"]),
            [[0, 0, 0, 3], [3, 3, 3, 6], [0, 0, 0, 3]],
        )

    def test_9(self):
        self.assertListEqual(
            final(10, 1, ["1r", "2r", "3r", "0c"]),
            [[1], [2], [2], [2], [1], [1], [1], [1], [1], [1]],
        )

    def test_10(self):
        self.assertListEqual(
            final(2, 5, ["1r", "1r", "1r", "1c", "0c", "0c", "1r", "0c", "1r", "0c"]),
            [[4, 1, 0, 0, 0], [9, 6, 5, 5, 5]],
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Incrementing Rows and Columns](https://edabit.com/challenge/8BQKa98d3s9Kis4vv)
