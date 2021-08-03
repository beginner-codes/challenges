# Challenge 303 - Sum of Other List Items

Create a function that is given a list of numbers and must return a list of the sum of all numbers from the original list except for the number at the current index.

## Example
```
[1, 2, 3, 4] = for first element => sum will be 2+3+4 = [9]
[1, 2, 3, 4] = for second element => sum will be 1+3+4 = [9, 8]
[1, 2, 3, 4] = for third element => sum will be 1+2+4 = [9, 8, 7]
[1, 2, 3, 4] = for fourth element => sum will be 1+2+3 = [9, 8, 7, 6]
```
## Examples
```python
lst_ele_sum([1, 2, 3, 2, 1]) ➞ [8, 7, 6, 7, 8]

lst_ele_sum([1, 2]) ➞ [2, 1]

lst_ele_sum([1, 2, 3]) ➞ [5, 4, 3]

lst_ele_sum([1, 2, 3, 4, 5]) ➞ [14, 13, 12, 11, 10]

lst_ele_sum([10, 20, 30, 40, 50, 60]) ➞ [200, 190, 180, 170, 160, 150]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def get_list_of_sums(lst: list[int]) -> list[int]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(get_list_of_sums([1, 2]), [2, 1])

    def test_2(self):
        self.assertListEqual(get_list_of_sums([1, 2, 3]), [5, 4, 3])

    def test_3(self):
        self.assertListEqual(get_list_of_sums([1, 2, 3, 4, 5]), [14, 13, 12, 11, 10])

    def test_4(self):
        self.assertListEqual(
            get_list_of_sums([10, 20, 30, 40, 50, 60]), [200, 190, 180, 170, 160, 150]
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Sum of List Elements Except Itself](https://edabit.com/challenge/93o8dzshnn2fDHdpX)
