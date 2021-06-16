# Challenge 269 - Length of a Nested List

The `len` function will return the number of items in a list. For example, the list below contains 2 items:
```python
[1, [2, 3]]
# 2 items, number 1 and list [2, 3]
```
Suppose we instead wanted to know the total number of non-nested items in the nested list. In the above case, `[1, [2, 3]]` contains 3 non-nested items: 1, 2 and 3.

Write a function that returns the total number of non-nested items in a nested array.

## Examples
```python
get_length([1, [2, 3]]) ➞ 3

get_length([1, [2, [3, 4]]]) ➞ 4

get_length([1, [2, [3, [4, [5, 6]]]]]) ➞ 6

get_length([1, [2], 1, [2], 1]) ➞ 5
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from typing import Any
import unittest


def get_length(lst: list[Any]) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(get_length([1, [2, 3]]), 3)

    def test_2(self):
        self.assertEqual(get_length([1, [2, [3, 4]]]), 4)

    def test_3(self):
        self.assertEqual(get_length([1, [2, [3, [4, [5, 6]]]]]), 6)

    def test_4(self):
        self.assertEqual(get_length([1, 7, 8]), 3)

    def test_5(self):
        self.assertEqual(get_length([2]), 1)

    def test_6(self):
        self.assertEqual(get_length([2, [3], 4, [7]]), 4)

    def test_7(self):
        self.assertEqual(get_length([2, [3, [5, 7]], 4, [7]]), 6)

    def test_8(self):
        self.assertEqual(get_length([2, [3, [4, [5]]], [9]]), 5)

    def test_9(self):
        self.assertEqual(get_length([]), 0)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Length of a Nested Array](https://edabit.com/challenge/yXSTvCNen2DQHyrh6)
