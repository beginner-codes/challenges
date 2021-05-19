# Challenge 249 - Sort the Unsortable

In this challenge you will be given a list similar to the following:
```python
[[3], 4, [2], [5], 1, 6]
```
In words, elements of the list are either an integer or a list containing a single integer. We humans can clearly see that this list can reasonably be sorted according to "the content of the elements" as:
```python
[1, [2], [3], 4, [5], 6]
```
Create a function that, given a list similar to the above, sorts the list according to the "content of the elements".

## Examples
```python
sort_it([4, 1, 3]) ➞ [1, 3, 4]

sort_it([[4], [1], [3]]) ➞ [[1], [3], [4]]

sort_it([4, [1], 3]) ➞ [[1], 3, 4]

sort_it([[4], 1, [3]]) ➞ [1, [3], [4]]

sort_it([[3], 4, [2], [5], 1, 6]) ➞ [1, [2], [3], 4, [5], 6]
```
## Notes

- To reiterate, elements of the list will be either integers or lists with a single integer.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from typing import Union
import unittest


def sort_it(unsorted_list: list[Union[list[int], int]]) -> list[Union[list[int], int]]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(sort_it([4, 1, 3]), [1, 3, 4])

    def test_2(self):
        self.assertEqual(sort_it([[4], [1], [3]]), [[1], [3], [4]])

    def test_3(self):
        self.assertEqual(sort_it([4, [1], 3]), [[1], 3, 4])

    def test_4(self):
        self.assertEqual(sort_it([[4], 1, [3]]), [1, [3], [4]])

    def test_5(self):
        self.assertEqual(sort_it([[3], 4, [2], [5], 1, 6]), [1, [2], [3], 4, [5], 6])

    def test_6(self):
        self.assertEqual(sort_it([[3], 7, [9], [5], 1, 6]), [1, [3], [5], 6, 7, [9]])

    def test_7(self):
        self.assertEqual(
            sort_it([[3], 7, [9], [5], 1, 6, [0]]), [[0], 1, [3], [5], 6, 7, [9]]
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Sort the Unsortable](https://edabit.com/challenge/zemLfbNWaKuhrbJPt)
