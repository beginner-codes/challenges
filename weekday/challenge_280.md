# Challenge 280 - Beginning and End Pairs

Write a function that pairs the first number in an array with the last, the second number with the second to last, etc.

## Examples
```python
pairs([1, 2, 3, 4, 5, 6, 7]) ➞ [[1, 7], [2, 6], [3, 5], [4, 4]]

pairs([1, 2, 3, 4, 5, 6]) ➞ [[1, 6], [2, 5], [3, 4]]

pairs([5, 9, 8, 1, 2]) ➞ [[5, 2], [9, 1], [8, 8]]

pairs([]) ➞ []
```
## Notes

- If the list has an odd length, repeat the middle element twice for the last pair.
- Return an empty list if the input is an empty list.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def pairs(sequence: list[int]) -> list[list[int]]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(pairs([1, 2, 3, 4, 5, 6, 7]), [[1, 7], [2, 6], [3, 5], [4, 4]])

    def test_2(self):
        self.assertListEqual(pairs([1, 2, 3, 4, 5, 6]), [[1, 6], [2, 5], [3, 4]])

    def test_3(self):
        self.assertListEqual(pairs([5, 9, 8, 1, 2]), [[5, 2], [9, 1], [8, 8]])

    def test_4(self):
        self.assertListEqual(pairs([1, 1, 4, 4, 5, 5]), [[1, 5], [1, 5], [4, 4]])

    def test_5(self):
        self.assertListEqual(pairs([9, 9, 9, 9, 3, 3, 9]), [[9, 9], [9, 3], [9, 3], [9, 9]])

    def test_6(self):
        self.assertListEqual(pairs([5, 6, 7]), [[5, 7], [6, 6]])

    def test_7(self):
        self.assertListEqual(pairs([5, 6]), [[5, 6]])

    def test_8(self):
        self.assertListEqual(pairs([5]), [[5, 5]])

    def test_9(self):
        self.assertListEqual(pairs([]), [])


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Beginning and End Pairs](https://edabit.com/challenge/HrCuzAKE6skEYgDmf)
