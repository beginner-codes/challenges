# Challenge 354 - Finding Common Elements

Create a function that takes two lists of numbers sorted in ascending order and returns a list of numbers which are common to both the input lists.

## Examples
```python
common_elements([-1, 3, 4, 6, 7, 9], [1, 3]) ➞ [3]

common_elements([1, 3, 4, 6, 7, 9], [1, 2, 3, 4, 7, 10]) ➞ [1, 3, 4, 7]

common_elements([1, 2, 2, 2, 3, 4, 5], [1, 2, 4, 5]) ➞ [1, 2, 4, 5]

common_elements([1, 2, 3, 4, 5], [10, 12, 13, 15]) ➞ []
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def common_elements(list_a: list[int], list_b: list[int]) -> list[int]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(common_elements([-1, 3, 4, 6, 7, 9], [1, 3]), [3])

    def test_2(self):
        self.assertListEqual(
            common_elements([1, 3, 4, 6, 7, 9], [1, 2, 3, 4, 7, 10]), [1, 3, 4, 7]
        )

    def test_3(self):
        self.assertListEqual(common_elements([-1, 3, 4, 6, 7, 9], []), [])

    def test_4(self):
        self.assertListEqual(
            common_elements([1, 2, 2, 2, 3, 4, 5], [1, 2, 4, 5]), [1, 2, 4, 5]
        )

    def test_5(self):
        self.assertListEqual(common_elements([-1, 3, 4, 6, 7, 9], [100, 300, 900]), [])
        

if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Finding Common Elements](https://edabit.com/challenge/E882au3CJba2jfQyT)
