# Challenge 406 - Moving Partition

Create a function to partition a list from left to right.

## Examples
```python
moving_partition([-1, -1, -1, -1])
➞ [[[-1], [-1, -1, -1]], [[-1, -1], [-1, -1]], [[-1, -1, -1], [-1]]]

moving_partition([1, 2, 3, 4, 5])
➞ [[[1], [2, 3, 4, 5]], [[1, 2], [3, 4, 5]], [[1, 2, 3], [4, 5]], [[1, 2, 3, 4], [5]]]

moving_partition([]) ➞ []
```
## Notes

- With an `n` input, your output should be a list containing `n-1` sublists. Each sublist should have two elements: the left and the right side of the partition (both should be non-empty, unless the input list is empty).
- An empty list should return an empty list: `[]`

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from typing import List
import unittest


Partition = List[List[int], List[int]]


def moving_partition(lst: list[int]) -> List[Partition]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(
            moving_partition([1, 2, 3, 4, 5]),
            [
                [[1], [2, 3, 4, 5]],
                [[1, 2], [3, 4, 5]],
                [[1, 2, 3], [4, 5]],
                [[1, 2, 3, 4], [5]],
            ],
        )

    def test_2(self):
        self.assertEqual(
            moving_partition([-1, -1, -1, -1]),
            [[[-1], [-1, -1, -1]], [[-1, -1], [-1, -1]], [[-1, -1, -1], [-1]]],
        )

    def test_3(self):
        self.assertEqual(moving_partition([8, 9, 10]), [[[8], [9, 10]], [[8, 9], [10]]])

    def test_4(self):
        self.assertEqual(moving_partition([]), [])


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Moving Partition](https://edabit.com/challenge/zYr4v5gb43kJPje9g)
