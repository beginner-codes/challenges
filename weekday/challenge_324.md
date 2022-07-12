# Challenge 324 - Odd Up, Even Down — N Times

Create a function that performs an even-odd transform to a list, `n` times. Each even-odd transformation:

- Adds two (+2) to each odd integer.
- Subtracts two (-2) from each even integer.

## Examples
```python
even_odd_transform([3, 4, 9], 3) ➞ [9, -2, 15]
# Since [3, 4, 9] => [5, 2, 11] => [7, 0, 13] => [9, -2, 15]

even_odd_transform([0, 0, 0], 10) ➞ [-20, -20, -20]

even_odd_transform([1, 2, 3], 1) ➞ [3, 0, 5]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def even_odd_transform(numbers: list[int], iterations: int) -> list[int]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(even_odd_transform([3, 4, 9], 3), [9, -2, 15])

    def test_2(self):
        self.assertListEqual(even_odd_transform([0, 0, 0], 10), [-20, -20, -20])

    def test_3(self):
        self.assertListEqual(even_odd_transform([1, 2, 3], 1), [3, 0, 5])

    def test_4(self):
        self.assertListEqual(even_odd_transform([55, 90, 830], 2), [59, 86, 826])


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Odd Up, Even Down — N Times](https://edabit.com/challenge/ke4FSMdG2XYxbGQny)
